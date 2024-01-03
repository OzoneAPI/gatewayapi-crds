# Gateway API CRDs

Deploys K8s Gateway API CRDs. No official Helm chart exists for this, this is a stopgap while its under [discussion](https://github.com/kubernetes-sigs/gateway-api/discussions/934)

Note that Helm is not the reccomended way to install CRDs, and has no capability to manage upgrades or remove old CRDs. However, consuming custom resource defitions like this can be helpful when bootstrapping a cluster. 

## Get started

Add this repository to Helm.

```
helm repo add gatewayapi-crds https://ozoneapi.github.io/gatewayapi-crds
```

Install an example.

```
helm install gatewayapi-crds-standard gatewayapi-crds/gatewayapi-crds-standard
```
