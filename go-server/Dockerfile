ARG OS
FROM ${OS} AS build

ENV BASE=${OS}

WORKDIR /app

COPY src ./ 

RUN CGO_ENABLED=0 go build -o main

CMD ["/app/main"]
