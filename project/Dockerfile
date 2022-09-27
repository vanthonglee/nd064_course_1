FROM python:3.8-slim-buster

WORKDIR /app

COPY ./techtrends/requirements.txt requirements.txt

RUN pip3 install -r requirements.txt 

COPY ./techtrends /app

RUN python3 init_db.py

EXPOSE 3111

CMD ["python", "app.py"]