FROM python:3.9-slim

# Set working directory
WORKDIR /workspace

# Install OS dependencies
RUN apt-get update && apt-get install -y \
    build-essential \
    curl \
    git \
    default-libmysqlclient-dev \
    libsasl2-dev \
    libpq-dev \
    && rm -rf /var/lib/apt/lists/*

# Upgrade pip
RUN pip install --upgrade pip setuptools wheel
