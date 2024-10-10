# backend_rds/Dockerfile
FROM python:3.9-slim

WORKDIR /app

# Install PostgreSQL development libraries for psycopg2
RUN apt-get update && apt-get install -y libpq-dev gcc

# Copy requirements and install dependencies
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copy the rest of the application
COPY . .

# Expose the necessary port
EXPOSE 8000

# Define the command to run the application
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]

