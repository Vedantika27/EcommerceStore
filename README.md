# My E-Commerce Store

A small static e-commerce demo website for the DevOps practical.

## Files
- `index.html` — website source code
- `Dockerfile` — Docker image configuration
- `.dockerignore` — files excluded from the Docker build context

## Run with Docker
Make sure Docker Desktop is running, then open a terminal in this folder:

```bash
docker build -t ecommerce-store .
docker run -d --name ecommerce-container -p 8080:80 ecommerce-store
```

Open http://localhost:8080

## Useful Docker commands
```bash
docker ps
docker stop ecommerce-container
docker rm ecommerce-container
```

## Upload to GitHub
Create an empty GitHub repository, then run:

```bash
git init
git add .
git commit -m "Initial e-commerce application"
git branch -M main
git remote add origin YOUR_GITHUB_REPOSITORY_URL
git push -u origin main
```
