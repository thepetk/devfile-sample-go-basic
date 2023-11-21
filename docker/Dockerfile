FROM registry.access.redhat.com/ubi9/go-toolset:1.18.9-14

COPY . .
RUN go mod download

RUN go build -o ./main

ENV PORT 8080
EXPOSE 8080

CMD [ "./main" ]
