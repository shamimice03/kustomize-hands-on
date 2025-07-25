# commands
```bash
kustomize build k8s

kustomize build k8s/ | kubectl apply -f -

kubectl apply -k k8s

kubectl delete -f k8s
```

# patch
- json 6902 patch

```
kustomize build patch-json6902
```

- strategic merge patch
```
kustomize build patch-strategic-merge-patch
```

## complete
```
k create -k overlays/prod
k create -k overlays/stg
```