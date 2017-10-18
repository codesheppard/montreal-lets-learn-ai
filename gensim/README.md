# About
This was the image for the meetup groups Gensim tutorial hosted on Oct. 18. 2017.

## Technical Details
This docker container was based off of the official miniconda3 environment. It subsequently runs some custom conda setup.

## Testing
- [x] Ran on Ubuntu 16.04 running Docker version 17.05.0-ce, build 89658be
- [x] Ran on Windows 10 Pro running Docker for Windows Docker version 17.09.0-ce, build afdb6d4

## Running

Linux/Mac
```
$> cd deep-learning/gensim
$> docker run --init -p 8888:8888 --mount type=bind,source="$(pwd)",target=/notebooks  -it mllai/gensim
```

Windows
```
# you will need to locate the path string to the embeddings folder and mount it

$> docker run --init -p 8888:8888 --mount type=bind,source="<FULL_PATH_TO_GENSIM>",target=/notebooks -it mllai/gensim
```
