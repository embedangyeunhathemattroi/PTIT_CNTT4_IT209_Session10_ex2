# Session 10 - Exercise 2: Single-stage Dockerfile

## Muc tieu
Dong goi ung dung Node.js Express REST API bang Docker.

## Cong nghe
- Node.js 18 Alpine
- Express.js
- Docker Desktop

## Build Docker Image
docker build -t hw-backend:v1 .

## Run Container
docker run -d --name app-single-stage -p 8080:3000 hw-backend:v1

## Kiem tra Container
docker ps
docker logs app-single-stage

## Kiem tra API
curl.exe -i http://localhost:8080/

## Ket qua mong doi
HTTP/1.1 200 OK

{"status":"success","message":"Hello from Docker Single-stage!"}

## Ket luan
Ung dung REST API duoc dong goi bang Single-stage Dockerfile.
