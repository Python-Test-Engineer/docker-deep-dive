
git clone https://github.com/pythonincontainers/smaller

cd smaller

atom .

docker build -t factors_flask:standard -f Dockerfile.standard .

docker run -it --rm -p 5000:5000 factors-flask:standard

Open Web browser with localhost:5000/65907657

substitute localhostwith Docker Machine IPaddress, if necessary.

docker images factors_flask$ docker images python:3.7.3

docker build -t factors_flask:slim -f Dockerfile.slim .

docker run -it --rm -p 5000:5000 factors_flask:slim

docker images factors_flask

docker build -t factors_flask:alpine -f Dockerfile.alpine .

docker run -it --rm -p 5000:5000 factors_flask:alpine

docker images factors_flask