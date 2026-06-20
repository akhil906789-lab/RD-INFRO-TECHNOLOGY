# Task 5 - Docker Containerization

## Objective

Containerize a simple web application using Docker and deploy it on an AWS EC2 instance.

---

## Tools Used

* AWS EC2
* Docker
* Ubuntu 24.04
* Nginx
* HTML

---

## Project Structure

```
Task-5-Docker
│
├── index.html
├── Dockerfile
├── README.md
├── Docker_Version.png
├── Dockerfile.png
├── Docker_Images.png
├── Docker_Container_Running.png
├── Website_Output.png
└── Repository_Structure.png
```

---

## HTML File

**index.html**

```html
<!DOCTYPE html>
<html>
<head>
    <title>Task 5 Docker</title>
</head>
<body>
    <h1>Docker Container Successfully Running</h1>
    <h2>RD INFRO TECHNOLOGY Internship</h2>
</body>
</html>
```

---

## Dockerfile

```dockerfile
FROM nginx:latest

COPY index.html /usr/share/nginx/html/index.html

EXPOSE 80
```

---

## Commands Used

### Install Docker

```bash
sudo apt update
sudo apt install docker.io -y
sudo systemctl start docker
docker --version
```

### Build Docker Image

```bash
sudo docker build -t task5-image .
```

### Verify Images

```bash
sudo docker images
```

### Run Docker Container

```bash
sudo docker run -d -p 80:80 --name task5-container task5-image
```

### Verify Running Container

```bash
sudo docker ps
```

---

## Website Output

The application was successfully deployed inside a Docker container and accessed through the EC2 public IP address.

Output displayed:

```
Docker Container Successfully Running

RD INFRO TECHNOLOGY Internship
```

---

## Screenshots Included

* Docker_Version.png
* Dockerfile.png
* Docker_Images.png
* Docker_Container_Running.png
* Website_Output.png
* Repository_Structure.png

---

## Conclusion

Successfully containerized a static HTML website using Docker, built the Docker image, launched the container, and accessed the application through an AWS EC2 instance.
