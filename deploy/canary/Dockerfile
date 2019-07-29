FROM golang:1.11
MAINTAINER vmarmol@google.com

RUN apt-get update && apt-get install -y git dmsetup && apt-get clean
RUN git clone https://gitlab.aibee.cn/rpzhang/cadvisor.git /go/src/gitlab.aibee.cn/rpzhang/cadvisor
RUN cd /go/src/gitlab.aibee.cn/rpzhang/cadvisor && make

ENTRYPOINT ["/go/src/gitlab.aibee.cn/rpzhang/cadvisor/cadvisor"]

