FROM ubuntu:focal

WORKDIR /app

RUN apt update && \
    apt-get install -y curl git build-essential && \
    DEBIAN_FRONTEND=noninteractive apt install -y software-properties-common && \
    apt-add-repository -y ppa:ansible/ansible && \
    apt update && apt install ansible -y 

COPY .bash_history /root/

CMD ["bash"]
