# ClusterIssuer Helm Chart for Jetstack's cert-manager

## Local Installation

```sh
helm install <release_name> . --namespace=<namespace> --set email=<your@email.com>
```

## Installation from Repository

```sh
helm repo add pacroy https://pacroy.github.io/helm-repo
```

```sh
helm repo update
```

```sh
helm install <release_name> pacroy/cluster-issuer --namespace=<namespace> --set email=<your@email.com> --set class=<nginx or traefik-cert-manager>
```
