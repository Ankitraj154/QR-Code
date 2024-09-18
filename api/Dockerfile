From python:3.9-slim

workdir /app

copy requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt

COPY . .

Expose 8000

CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000"]