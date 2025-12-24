# Running Ollama and Open WebUI in a Kubernetes Cluster


Running Ollama and Open WebUI in a Kubernetes Cluster

## Prerequisite

- Docker Desktop
- Enable Kubernetes under Settings > Kubernetes

## Clone the repository

```
git clone https://github.com/arunudaiyar/openweb-ollama-k8s.git
cd openweb-ollama-k8s
```

## Apply the Kubernetes Manifest

```
kubectl apply -f ./
```


## Accessing the Open Web UI

```
kubectl port-forward svc/svc-open-webui 8080:8080 -n ollama
```

## Open Open WebUI

Open [http://localhost:8080](http://localhost:8080) to access Open WebUI.

<img width="1366" height="645" alt="openweb-llama" src="https://github.com/user-attachments/assets/354127e4-4ffb-4503-986d-c6103da81f47" />

