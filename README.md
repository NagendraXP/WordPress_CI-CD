## Usage

### Local Development Environment

```bash
# Clone the repo
git clone https://github.com/NagendraXP/WordPress_CI-CD.git
cd WordPress_CI-CD

# Spin it up with Docker Compose
docker compose up -d

# Open your browser and head to http://localhost:8080
# You will find the famous WordPress 5-minute install
```

### Kubernetes

```bash
# Deploy with kubectl
kubectl apply -f https://github.com/NagendraXP/WordPress_CI-CD/master/deploy/kubernetes/deploy.yaml

# The namespace 'WordPress_CI-CD' is created to host the example resources:
# - 1 Stateful MySQL replica with emptyDir volume (data lost on restart)
# - 3 Stateless WordPress replicas (horizontal scaling)
# - A Secret storing WordPress Enviroment Configuration
# - A Service with type LoadBalancer to expose the app

# Open your browser and head to the service External IP
# You will find the WordPress
```


