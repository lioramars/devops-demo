# devops-demo

This is a simple DevOps demo project designed to showcase a full CI/CD workflow using:

- **Docker**
- **NGINX**
- **GitHub Actions**
- **Docker Hub**

Every time a change is pushed to the `main` branch, GitHub Actions automatically:
1. Builds a new Docker image  
2. Logs into Docker Hub  
3. Pushes the updated image to the repository:  
   `lior98/devops-demo:latest`

---

## 🚀 Run Locally

To run this project locally using Docker:

### 1. Pull the latest image from Docker Hub:
```bash
docker pull lior98/devops-demo:latest
RUN:
docker run -p 5000:80 lior98/devops-demo:latest
and go to:
http://localhost:5000

