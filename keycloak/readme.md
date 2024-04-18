We require that nginx ingress and cert-manager are installed and configured

Values.yaml is for bitnami keycloak helm chart.
Usage:
```
helm install keycloak bitnami/keycloak -f values.yaml -n [NAMESPACE]
```
```
kubectl apply -f nginx-ingress-config.yaml -n [NAMESPACE]
```

After deploy check if ingress gets ip
```
kubectl get ingress -n [NAMESPACE]
```

