# N8N Example

This project sets up [n8n](https://n8n.io) — a powerful open-source workflow automation tool — using **Docker Compose** with a **PostgreSQL** database for persistent and scalable storage.

## How to Run (Local)

### 1. Clone Repo

```shell
git clone git@github.com:agung96tm/n8n-example.git
cd n8n-example
```

### 2. Copy Envs
```shell
copy deploy/.env.example deploy/.env
copy deploy/.db-env.example deploy/.db-env
```

### 3. Run Service
```shell
docker-compose up -d
```


### 4. Access
```shell
http://localhost:5678
```
> If you enabled basic auth in the environment variables, use the username/password set in the .env or docker-compose.yml.


## How to Run (k8s)
```shell
copy deploy/k8s-env.example deploy/k8s/k8s-env.yaml
kubectl apply -f deploy/k8s
```


## References
- [Official: n8n - Community](https://docs.n8n.io/hosting/community-edition-features/#registered-community-edition)

## Contributors
- [Agung Yuliyanto](https://github.com/agung96tm)
