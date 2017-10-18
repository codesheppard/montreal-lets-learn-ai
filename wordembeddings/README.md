# About
This was the image for the meetup groups Wordembeddings tutorial hosted on Oct. 18. 2017.

## Technical Details
This docker container was based off of the official miniconda3 environment. It subsequently runs the Udacity setup
environment.

We subsequently installed the
[requirements.txt](https://github.com/udacity/deep-learning/commit/8e9be5fcfe67bbedd00f51a5016732988d2d13fb)
for the Udacity Deep Learning repository.

## Testing
- [x] Ran on Ubuntu 16.04 running Docker version 17.05.0-ce, build 89658be
- [ ] Ran on Windows 10 Pro running Docker for Windows

## Running

Linux/Mac
```
$> cd deep-learning/wordembeddings
$> docker run -p 8888:8888 --mount type=bind,source="$(pwd)",target=/notebooks  -it mllai/wordembeddings
```

Windows
```
# you will need to locate the path string to the embeddings folder and mount it

$> docker run --init -p 8888:8888 --mount type=bind,source="<FULL_PATH_TO_EMBEDDINGS>",target=/notebooks -it mllai/wordembeddings
```
