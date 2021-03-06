## helm verify

verify that a chart at the given path has been signed and is valid

### Synopsis



Verify that the given chart has a valid provenance file.

Provenance files provide crytographic verification that a chart has not been
tampered with, and was packaged by a trusted provider.

This command can be used to verify a local chart. Several other commands provide
'--verify' flags that run the same validation. To generate a signed package, use
the 'helm package --sign' command.


```
helm verify [flags] PATH
```

### Options

```
      --keyring string   keyring containing public keys (default "~/.gnupg/pubring.gpg")
```

### Options inherited from parent commands

```
      --debug                           enable verbose output
      --home string                     location of your Helm config. Overrides $HELM_HOME (default "~/.helm")
      --host string                     address of Tiller. Overrides $HELM_HOST
      --kube-context string             name of the kubeconfig context to use
      --kubeconfig string               absolute path to the kubeconfig file to use
      --tiller-connection-timeout int   the duration (in seconds) Helm will wait to establish a connection to tiller (default 300)
      --tiller-namespace string         namespace of Tiller (default "kube-system")
      --tls                             enable TLS connection between Helm and Tiller
      --tls-ca-cert string              path to TLS CA certificate file used to verify the Helm client and Tiller server certificates
      --tls-cert string                 path to Helm TLS client certificate file for authenticating to Tiller
      --tls-key string                  path to Helm TLS client key file for authenticating to Tiller
      --tls-verify                      enable TLS connection between Helm and Tiller and verify Tiller server certificate
```

### SEE ALSO
* [helm](helm.md)	 - The Helm package manager for Kubernetes.

###### Auto generated by spf13/cobra on 27-Jul-2018
