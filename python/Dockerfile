FROM linuxserver/code-server:4.16.1

RUN sudo apt-get update
RUN sudo apt-get install software-properties-common -y
RUN sudo add-apt-repository ppa:deadsnakes/ppa
RUN sudo apt-get update
RUN sudo apt-get install python3.8 -y

RUN sudo apt install virtualenv -y
