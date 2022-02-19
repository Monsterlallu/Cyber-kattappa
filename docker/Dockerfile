FROM golang:1-alpine
LABEL maintainer="Alexander I.Grafov <grafov@gmail.com>"

RUN apk add --no-cache git \
  && go get -d -v github.com/Monsterlallu/Cyber-kattappa \
  && go install github.com/Monsterlallu/Cyber-kattappa/hulk@latest \
  && rm -rf ~/go/src/github.com/Monsterlallu/Cyber-kattappa \
  && apk del git

ENTRYPOINT ["Cyber-kattappa"]

CMD ["--help"]
