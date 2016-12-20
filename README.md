# docker-ffmpeg
An FFmpeg Dockerfile from source. Built on Alpine Linux.

* ffmpeg 3.1.5 (compiled from source)

[![Docker Stars](https://img.shields.io/docker/stars/alfg/ffmpeg.svg)]()
[![Docker Pulls](https://img.shields.io/docker/pulls/alfg/ffmpeg.svg)]()
[![Docker Automated build](https://img.shields.io/docker/automated/alfg/ffmpeg.svg)]()
[![Build Status](https://travis-ci.org/alfg/docker-ffmpeg.svg?branch=master)](https://travis-ci.org/alfg/docker-ffmpeg)

## Usage
```
docker build -t ffmpeg .
docker run -it ffmpeg ffmpeg -buildconf
```

or use as a base image in your Dockerfile:
```
FROM alfg/ffmpeg:latest
```

### FFmpeg Build
```
ffmpeg version 3.1.5 Copyright (c) 2000-2016 the FFmpeg developers
  built with gcc 5.3.0 (Alpine 5.3.0)
  configuration: --enable-version3 --enable-gpl --enable-nonfree --enable-small --enable-libmp3lame --enable-libx264 --enable-libx265 --enable-libvpx --enable-libtheora --enable-libvorbis --enable-libopus --enable-libfdk-aac --enable-libass --enable-libwebp --enable-librtmp --enable-postproc --enable-avresample --enable-libfreetype --enable-openssl --disable-debug
  libavutil      55. 28.100 / 55. 28.100
  libavcodec     57. 48.101 / 57. 48.101
  libavformat    57. 41.100 / 57. 41.100
  libavdevice    57.  0.101 / 57.  0.101
  libavfilter     6. 47.100 /  6. 47.100
  libavresample   3.  0.  0 /  3.  0.  0
  libswscale      4.  1.100 /  4.  1.100
  libswresample   2.  1.100 /  2.  1.100
  libpostproc    54.  0.100 / 54.  0.100

  configuration:
    --enable-version3
    --enable-gpl
    --enable-nonfree
    --enable-small
    --enable-libmp3lame
    --enable-libx264
    --enable-libx265
    --enable-libvpx
    --enable-libtheora
    --enable-libvorbis
    --enable-libopus
    --enable-libfdk-aac
    --enable-libass
    --enable-libwebp
    --enable-librtmp
    --enable-postproc
    --enable-avresample
    --enable-libfreetype
    --enable-openssl
    --disable-debug
```

## Resources
* https://alpinelinux.org/
* https://www.ffmpeg.org

## License
MIT