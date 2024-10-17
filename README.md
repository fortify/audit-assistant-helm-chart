Audit Assistant Helm charts repository
======================================

This repository contains the Fortify Audit Assistant Helm charts. It features a directory for each
Audit Assistant release (for example `24.4.0`). The release directory contains Helm chart packages
for the release and an example of chart configuration file named `custom-values-example.yaml`.

A Helm chart package (`audit-assistant-<CHART_VERSION>.tgz`) can be downloaded and used locally as follows:

```sh
# deploy Audit Assistant from a local chart package
helm install <NAME> ./audit-assistant-<CHART_VERSION>.tgz ...
```

Additionally, valid metadata for a Helm chart repository are included allowing use with Helm as follows:

```sh
# add remote Helm chart repository named "fortify"
helm repo add fortify https://raw.githubusercontent.com/fortify/audit-assistant-helm-charts/repo/

# list all chart versions in "fortify" repository
helm search repo fortify/

# deploy Audit Assistant from a remote chart package
helm install <NAME> fortify/audit-assistant --version <CHART_VERSION> ...
```

Please refer to [Audit Assistant documentation](https://www.microfocus.com/documentation/fortify-audit-assistant/) for full instructions.
