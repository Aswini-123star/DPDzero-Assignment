ASSIGNMENT:

This project contains:
.
├── docker-compose.yml
├── ngnix
│   ├── Dockerfile
│   └── nginx.conf
├── service_1
│   ├── Dockerfile
│   ├── README.md
│   └── main.go
└── service_2
    ├── Dockerfile
    ├── README.md
    ├── app.py
    ├── pyproject.toml
    └── uv.lock

service_1:[Golang]
1) Go to service_1 folder 
run go run main.go
2) Dockerfile -> build the docker image -> container
3) Port number 8001:8001
4) Check the services:
5) Open in chrome -> 13.61.2.39:8001/ping
6) Open in chrome -> 13.61.2.39:8001/hello

service_2:[Python]
1)Go to the service_2 folder.
2)Install dependencies with uv or pip.
uv run app.py
3)Dockerfile -> build docker image -> container
4)Port number 8002:8002
Check the services:
5)Open in chrome -> 13.61.2.39:8002/ping
6)Open in chrome -> 13.61.2.39:8002/hello

NGNIX:
Go to ngnix folder
NGNIX DIRECTORY -> ngnix.conf
Dockerfile -> build a docker image

By using the docker-compose up --build 
create a docker-compose.yml 
