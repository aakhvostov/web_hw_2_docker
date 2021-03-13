FROM python:latest

WORKDIR /code

COPY requirements.txt .

RUN pip install -r requirements.txt

COPY first_project.py .

CMD ["python", "first_project.py"]
