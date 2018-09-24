FROM debian:latest
RUN apt-get update -y
RUN apt-get install -y python-pip python-dev build-essential
RUN adduser user
COPY . /app
WORKDIR /app
RUN pip install -r requirements.txt
USER user
ENTRYPOINT ["python"]
CMD ["app.py"]