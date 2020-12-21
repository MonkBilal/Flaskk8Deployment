FROM python:alpine3.7 

WORKDIR /app


COPY . /app/

RUN pip install --upgrade pip &&\
    pip install -r requirements.txt &&\
    apk add --no-cache --virtual curl

EXPOSE 4000

CMD ["gunicorn", "-w", "4", "-b", "0.0.0.0:4000", "hello_world:APP"]
