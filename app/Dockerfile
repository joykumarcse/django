# base image
FROM python:3.9.7-buster

# options
ENV PYTHONUNBUFFERED 1

# Set working directory
RUN mkdir /app
WORKDIR /app

# Copy requirements file
COPY requirements.txt .

# Install Python packages
RUN pip install --upgrade pip && \
    pip install -r requirements.txt

# Copy the rest of the application code
COPY . .

# Expose the necessary port
EXPOSE 8000

# Specify the command to run the Django development server
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]

