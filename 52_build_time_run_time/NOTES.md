https://github.com/pythonincontainers/buildtime-runtime

git clone https://github.com/pythonincontainers/buildtime-runtime

cd buildtime-runtime$ atom .

docker built -t runtime -f Dockerfile.runtime .

docker run -it --rm -p 8000:8000 runtime

docker run -it --rm -p 8000:8000 runtime

docker run -it --name runtime -p 8000:8000 runtime$ docker start -ai runtime

docker rm -f runtime

docker build -t runtime -f Dockerfile.runtime .

docker run -it --rm -p 8000:8000 runtime$ docker run -it --rm -p 8000:8000 -e DJANGO_VER=2.1.8 runtime

docker build -t buildtime -f Dockerfile.buildtime 

docker volume create buildtime-vol$ docker run -it --rm -v buildtime-vol:/data -p 8000:8000 buildtime$ docker run -it --rm -v buildtime-vol:/data -p 8000:8000 buildtime


docker build -t buildtime -f Dockerfile.buildtime –build-arg Django=2.2.1 .

docker run -it --rm -p 8000:8000 python:3.7.3 bash -c "git clone https://github.com/pythonincontainers/buildtime-runtime /django-mysite; cd django-mysite; bash run-server.sh