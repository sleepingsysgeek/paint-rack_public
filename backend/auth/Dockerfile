from python:3.13
Workdir /app
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt
COPY ./app ./app
expose 8000
cmd ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "10000"]
