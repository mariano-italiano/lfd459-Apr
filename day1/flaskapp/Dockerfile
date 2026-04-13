FROM python:3.10-slim-buster

MAINTAINER Marcin Kujawski

WORKDIR /app

COPY requirements.txt .

RUN pip3 install --no-cache-dir -r requirements.txt

RUN adduser flaskuser

COPY --chown=flaskuser:flaskuser . .

RUN chmod -R 755 .

USER flaskuser

ENV PYTHONVAR="/test/path"

CMD ["python3", "app.py"]
