# Kubeconfig

This is and example of the `kubeconfig` to use with `opencp` or open control plane, you only ed replace `<TOKER>` by your provider token

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

