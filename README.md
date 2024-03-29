# theloungue-k8s
Kubernetes manifests for The Lounge IRC client

### Installation
`kubectl apply -f dist/`

### Expose service (optional)
`kubectl port-forward --address [external_address] -n thelounge service/thelounge-service 8000:80`

### Create username and password
`kubectl exec --user node -it [pod_name] thelounge add [username]`

### Open The Lounge
http://[external_address]:8000
