# Pull base image
FROM python:3.7-slim

# Set environment variables
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONBUFFERED 1

# Set work directory
WORKDIR /code

# Install dependencies
# COPY Pipfile.lock /code/
ADD Pipfile* /code/
RUN pip install pipenv && pipenv install --system

# Copy project
COPY . /code/
