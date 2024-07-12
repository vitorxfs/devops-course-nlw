# Kubernetes

add `secret.yaml` with:

```yaml
apiVersion: v1
kind: Secret
metadata:
  name: db-connection
type: Opaque
data:
  db_user:
  db_password:
  db_host:
  db_port:
  db_name:
```

then, run the following command:

```sh
kubectl apply -f k8s/secret.yaml -n <namespace>
```
