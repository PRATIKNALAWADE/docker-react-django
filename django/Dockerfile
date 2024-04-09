FROM python:3.8-alpine
ENV PYTHONUNBUFFERED 1

# Update package lists
RUN apk update

# Install build tools including gcc
RUN apk add gcc build-base
WORKDIR /django
COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt
COPY . .