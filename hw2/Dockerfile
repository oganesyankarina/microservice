FROM python:3.9

# WORKDIR /app

COPY requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt

ADD . /app

# COPY . .

EXPOSE 8080

RUN apt update

# CMD ["python", "./app.py"]
ENTRYPOINT python /app/app.py runserver 0.0.0.0:8080
