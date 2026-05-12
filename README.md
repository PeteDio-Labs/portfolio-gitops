# portfolio-gitops

GitOps manifests for [petedillo.com](https://petedillo.com) portfolio.

Watched by ArgoCD app `portfolio` (defined in `petedio-labs-gitops/argocd/applications/portfolio.yaml`).

## Layout

- `kubernetes/base/` — Deployment, Service, Ingress
- `kubernetes/overlays/prod/` — production overlay (namespace + image tag)

ArgoCD Image Updater writes new image digests back to this repo on `main`.
