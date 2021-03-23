# Wordpress

## Usage

```console
argocd app create wordpress \
    --repo https://github.com/minchao/cd-example-apps.git \
    --path wordpress \
    --dest-server https://kubernetes.default.svc \
    --dest-namespace default \
    --helm-set wordpress.service.port=8080 \
    --helm-set wordpress.service.httpsPort=8443
```
