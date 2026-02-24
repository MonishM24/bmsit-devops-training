# Exercise 4: Dockerfile for a Python App

## Objective
Containerize a basic Python application and publish the image.

## What You Will Practice
- Writing a simple Python app
- Creating a Dockerfile
- Building and running a container image
- Pushing to Docker Hub

## Step 1: Create `app.py`
```python
print("Hello from Docker")
```

## Step 2: Create `Dockerfile`
```dockerfile
FROM python:3.9
WORKDIR /app
COPY app.py .
CMD ["python", "app.py"]
```

## Step 3: Build, Push, and Run
```bash
docker build -t yourusername/python-app .
docker login
docker push yourusername/python-app
docker run yourusername/python-app
```

## Notes
- Replace `yourusername` with your Docker Hub username.
