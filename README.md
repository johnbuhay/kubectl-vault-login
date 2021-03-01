# kubectl-vault-login

Make it easier to authenticate oneself as a Kubernetes ServiceAccount to Vault

```text
-n|--namespace (optional) the namespace where the service account is located, otherwise use value set in context if it exists by default
-sa|--serviceaccount (required) the Service Account name to identify as
--role (required) the Vault role to authorize with
--context (optional) the kubeconfig context to target requests to, otherwise current-context in the kubeconfig
--kubeconfig (optional) explicitly set the location of the kubeconfig file to use, otherwise $KUBECONFIG or $HOME/.kube/config by default
--config (optional) explicitly set the location of the config file to use, otherwise $VAULTLOGIN_CONFIG or $HOME/.vault/login.yml by default
```

## Install
Add the executable in a directory that is listed in your $PATH as `kubectl-vault-login`

## Usage
```bash
kubectl vault-login --help


```

```bash
VAULTLOGIN_LOGLEVEL=verbose kubectl vault-login
Using vaultconfig $HOME/.vault/login.yml
Using kubeconfig $HOME/.kube/config
Using serviceaccount default in ns/default context/clustername
Successfully logged in with role X, you have Y minutes before expiration
```

## [To Do](./TODO.md)

> This project is licensed under the terms of the [Apache 2.0 License](./LICENSE.txt)
