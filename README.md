# Proyecto-Flux
Suspendido termporalmente para no saturar el cluster de MiniKube.

flux suspend kustomization apps -n flux-system
kubectl delete namespace demo

Para reanudar el proyecto, ejecutar:

kubectl create namespace demo
flux resume kustomization apps -n flux-system
flux reconcile kustomization apps -n flux-system --with-source