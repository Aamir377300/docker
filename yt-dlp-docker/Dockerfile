FROM python:3.11-slim

RUN apt-get update && apt-get install -y \
    curl \
    ffmpeg \
    && rm -rf /var/lib/apt/lists/*

RUN pip install --no-cache-dir yt-dlp

# Make a folder to store downloads inside the container
RUN mkdir /downloads

WORKDIR /downloads