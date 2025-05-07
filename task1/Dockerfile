# Use an official Python base image
FROM python:3.8-slim-buster

# Set the working directory inside the container
WORKDIR /app

# Copy the Python file into the container
COPY api.py /app/api.py

# Remove the EXTERNALLY-MANAGED file to avoid pip installation errors
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED || true

# Update the package list and install Python3 and pip3
RUN apt-get update -y && apt-get install -y python3 python3-pip

# Install Flask using pip3
RUN pip3 install flask

# Expose port 5252 for the Flask app
EXPOSE 5252

# Command to run the Flask app
CMD ["python3", "api.py"]