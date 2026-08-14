# Project2-notesapp-devops

## Kubernetes Secrets

Always add this file to `.gitignore`.

Apply the secret separately:

```bash
kubectl apply -f "secrets.yml"
```

### secrets.yml

```yaml
apiVersion: v1
kind: Secret
metadata:
  name: secret
  namespace: project-2
type: Opaque
data:
  MYSQL_PASSWORD: bml0aGlu  # Base64 encoded value of nithin
```

### .gitignore

```gitignore
extra k8's/secrets.yml
```