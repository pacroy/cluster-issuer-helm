# ClusterIssuer Helm Chart for Jetstack's cert-manager

[![Lint Code Base](https://github.com/pacroy/cluster-issuer-helm/actions/workflows/linter.yml/badge.svg)](https://github.com/pacroy/cluster-issuer-helm/actions/workflows/linter.yml) [![Test and Publish Chart](https://github.com/pacroy/cluster-issuer-helm/actions/workflows/test-and-publish.yml/badge.svg)](https://github.com/pacroy/cluster-issuer-helm/actions/workflows/test-and-publish.yml)

## Local Installation

```sh
helm upgrade --install <release_name> . --namespace=<namespace> --set email=<your@email.com>
```

## Installation from Repository

```sh
helm repo add pacroy https://pacroy.github.io/helm-repo
helm repo update
helm upgrade --install <release_name> pacroy/cluster-issuer --namespace=<namespace> --set email=<your@email.com> --set class=<nginx or traefik-cert-manager>
```
