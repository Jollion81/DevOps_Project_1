# backend_redis/Dockerfile
FROM python:3.9-slim

WORKDIR /app

# Copy requirements and install dependencies
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copy the rest of the application
COPY . .

# Expose the necessary port
EXPOSE 8001

# Define the command to run the application
CMD ["python", "manage.py", "runserver", "0.0.0.0:8001"]
