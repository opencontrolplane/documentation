# Kubeconfig

This is an example of the `kubeconfig` to use with OpenCP. The configuration is set to communicate with Civo's `LON1` region. To access resources in your account for that region, you would need to replace `<TOKEN>` with your provider token / API key, found on your Civo account profile.

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

