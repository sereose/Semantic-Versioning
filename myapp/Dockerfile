# Use an official Python runtime as the base image
FROM python:3.9-slim

# Set the working directory in the container
WORKDIR /app

# Copy the requirements file to the working directory
COPY myapp/requirements.txt .

# Install the app dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy the app code to the working directory
COPY app.py .

# Expose the desired port
EXPOSE 5000

# Define the command to run your app
CMD ["python", "app.py"]