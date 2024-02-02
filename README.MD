# build
```bash
docker build -t jscat/ffmpeg .
```

# build multi platform
```bash
docker buildx build --platform linux/amd64,linux/arm64 -t jscat/ffmpeg:latest --push .
```

# run
```bash
docker run --rm -it \
    -v $(pwd):/app -w /app \
    jscat/ffmpeg --help
```

# install docker
https://docs.docker.com/engine/install/ubuntu/
```bash
curl -fsSL https://get.docker.com -o get-docker.sh
sudo sh get-docker.sh
```

ffmpeg documentation: https://ffmpeg.org/ffmpeg.html