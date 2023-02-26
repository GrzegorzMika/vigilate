FROM golang:1.20

WORKDIR pusher

RUN apt-get install git -y
RUN git clone https://github.com/dimiro1/ipe.git && cd ipe/cmd && go build -o ipe

COPY config.yml config.yml

CMD /go/pusher/ipe/cmd/ipe