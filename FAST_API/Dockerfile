FROM ubuntu

RUN apt update -y
RUN apt install python3 python3-pip pip -y

WORKDIR /app
COPY . /app/
RUN pip install -r requirements.txt

EXPOSE 80


# CMD pipenv run uvicorn main:app --host 0.0.0.0 --port 80
CMD pip run python3 ./main.py