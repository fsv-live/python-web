FROM python:3.10.0
EXPOSE 5000
COPY requirements.txt .
RUN python -m pip install -r requirements.txt
WORKDIR /app
COPY . /app
CMD ["gunicorn", "--bind", "0.0.0.0:5000", "index:app"]