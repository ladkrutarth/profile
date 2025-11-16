# Krutarth Lad - Portfolio Website

Professional portfolio website showcasing my experience as a Data Scientist and Cloud Infrastructure Specialist.

## Technologies Used
- HTML5
- CSS3
- Docker
- Nginx

## Local Development

### Prerequisites
- Docker installed on your machine

### Run Locally with Docker

1. Clone this repository:
```bash
git clone https://github.com/YOUR_USERNAME/portfolio-website.git
cd portfolio-website
```

2. Build the Docker image:
```bash
docker build -t krutarth-portfolio .
```

3. Run the container:
```bash
docker run -d -p 8080:80 --name my-portfolio krutarth-portfolio
```

4. Open your browser and visit:
```
http://localhost:8080
```

### Stop the container:
```bash
docker stop my-portfolio
docker rm my-portfolio
```

## Deployment Options

### Option 1: Docker Hub
```bash
# Tag the image
docker tag krutarth-portfolio YOUR_DOCKERHUB_USERNAME/krutarth-portfolio:latest

# Push to Docker Hub
docker push YOUR_DOCKERHUB_USERNAME/krutarth-portfolio:latest

# Others can pull and run
docker pull YOUR_DOCKERHUB_USERNAME/krutarth-portfolio:latest
docker run -d -p 8080:80 YOUR_DOCKERHUB_USERNAME/krutarth-portfolio:latest
```

