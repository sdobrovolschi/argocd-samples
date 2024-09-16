### Recovering From an Existing Repository
To recover the Argo CD installation run:
```bash
export GIT_REPO=<REPO_URL>
export GIT_TOKEN=<YOUR_TOKEN>

argocd-autopilot repo bootstrap --recover
```

### Apply Argo-CD Manifests From Existing Repository
To apply the modified Argo CD manifests run:
```bash
export GIT_REPO=<REPO_URL>
export GIT_TOKEN=<YOUR_TOKEN>

argocd-autopilot repo bootstrap --recover --app "${GIT_REPO}.git/bootstrap/argo-cd"
```