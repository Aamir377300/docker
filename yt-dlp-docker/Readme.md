<!-- build the image -->

docker build -t yt-dlp-image .

<!-- run the command which dowload the video in the dowload -->
docker run --rm \
  -v "$(pwd):/downloads" \
  yt-dlp-image \
  yt-dlp -o "/downloads/%(title)s.%(ext)s" -a /downloads/url.txt