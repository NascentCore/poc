FROM ubuntu:16.04
FROM tensorflow/tensorflow
#COPY src /src
#WORKDIR /src
RUN mkdir -p cifar10
WORKDIR cifar10
RUN apt-get update && apt-get install -y wget
RUN wget -c https://www.cs.toronto.edu/~kriz/cifar-10-python.tar.gz
RUN tar -xvzf cifar-10-python.tar.gz
RUN rm cifar-10-python.tar.gz
