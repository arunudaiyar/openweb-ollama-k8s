# Running Ollama and Open WebUI in a Kubernetes Cluster


Running Ollama and Open WebUI in a Kubernetes Cluster

## Prerequisite

- Docker Desktop
- Enable Kubernetes under Settings > Kubernetes

## Clone the repository

```
git clone https://github.com/ajeetraina/ollama-openwebui-kubernetes
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

<img width="1185" alt="image" src="https://github.com/user-attachments/assets/e63a6d5d-9655-4ed2-b39b-2db019eca626">

## Pull a model

<img width="655" alt="image" src="https://github.com/user-attachments/assets/243fd811-b382-41c0-9e54-febc636c646b">

## Configuration Setting

Disable OpenAI and enable Ollama configuration by modifying it to http://localhost:11434

<img width="1236" alt="image" src="https://github.com/user-attachments/assets/ea8f0e9c-4d45-4980-ab54-9b93ce2a588b">
