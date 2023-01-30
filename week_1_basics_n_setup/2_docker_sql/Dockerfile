FROM python:3.9.1

RUN apt-get update
RUN apt-get install wget
RUN apt install python3-pip -y
RUN pip install pandas sqlalchemy psycopg2

WORKDIR /app
COPY ingest_data.py pipeline.py ./
ENTRYPOINT [ "python" , "pipeline.py"]