# Kubeconfig

This is an example of the `kubeconfig` to use with `opencp` or open control plane. You would need to replace `<TOKEN>` with your provider token / API key.

```yaml
apiVersion: v1
clusters:
  - cluster:
      server: https://opencp.lon1.civo.com
    name: kubernetes
contexts:
  - context:
      cluster: kubernetes
      user: admin
    name: opencp-lon
current-context: opencp-lon
kind: Config
preferences: {}
users:
  - name: admin
    user:
      token: <TOKEN>
```

