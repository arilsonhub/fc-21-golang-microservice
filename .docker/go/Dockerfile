FROM golang:1.24.0-bullseye

RUN apt-get update && apt-get install -y build-essential

WORKDIR /app

COPY . .

RUN go mod download

CMD [ "go", "run", "./cmd/trade/main.go" ]