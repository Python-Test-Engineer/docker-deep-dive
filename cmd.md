# 1

docker build -t args -f Dockerfile.arg --build-arg Flask_Ver=3.0 --build-arg Python_Image_Tag=3.12 .

docker run -it --rm -p 5000:5000 args

docker inspect args

# 2