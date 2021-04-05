# argo-gitops

## Usage

```console
kustomize build ./ | kubectl apply -f -
```

```console
argocd app create argo-gitops \
    --repo https://github.com/minchao/cd-example-apps.git \
    --path argo-gitops \
    --dest-server https://kubernetes.default.svc \
    --dest-namespace argocd
```