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


## References:
- https://notes.kodekloud.com/docs/Certified-Kubernetes-Application-Developer-CKAD/2025-Updates-Kustomize-Basics/Components 

- https://kubernetes.io/docs/tasks/manage-kubernetes-objects/kustomization/

- https://kubectl.docs.kubernetes.io/references/kustomize/