Section 3. „Parametrizing Dockerfile with ARG”Links:https://github.com/pythonincontainers/dockerfile-argCommands:$ 

git clone https://github.com/pythonincontainers/dockerfile-arg

cd dockerfile-arg$ atom .

docker build -t args -f Dockerfile.arg --build-arg Flask_Ver=1.0.0 .$ docker build -t args -f Dockerfile.arg --build-arg Flask_ver=1.0.0 --build_arg Python_Image_Tag=slim.

docker run -it --rm -p 5000:5000 args

docker build -t args -f Dockerfile.arg --build-arg Flask_Ver=1.0.0 --build-arg Python_Image_Tag=3.8.0a4-stretch .

docker run -it --rm -p 5000:5000 args$ docker inspect args

docker history args$ docker build -t args -f Dockerfile.env --build-arg Python_Image_Name=centos/python-36-centos7 .

docker run -it --rm -p 5000:5000 args