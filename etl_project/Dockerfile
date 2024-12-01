# Base image
FROM python:3.9-slim

# Maintainer information
LABEL maintainer="nombre.tu.email@example.com"

# Set the working directory
WORKDIR /app

# Install necessary libraries
COPY requirements.txt requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Copy the project files into the container
COPY . .

# Set the default command to run the ETL script
CMD ["python", "run_etl.py"]
