# PBS-Matrix

This repo contains the deployment config for Element Server Suite Community, which is an implemnetation of a Chat Service based on Matrix Protocol.

## Update/Install

```bash
kubectl apply -f secrets.yml
# Edit secrets to have content
helm upgrade --install --namespace "pbs-matrix" ess oci://ghcr.io/element-hq/ess-helm/matrix-stack -f values.yml --wait
```