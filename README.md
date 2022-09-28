# helm-charts
Helm chart repository

## Usage

[Helm](https://helm.sh) must be installed to use the charts.  Please refer to
Helm's [documentation](https://helm.sh/docs) to get started.

Once Helm has been set up correctly, add the repo as follows:
```bash
  helm repo add helium https://heliumplusemr.github.io/helm-charts
```

If you had already added this repo earlier, run `helm repo update` to retrieve
the latest versions of the packages.  You can then run `helm search repo
helium` to see the charts.

### To install the helium chart:
```bash
  helm install helium helium/helium
```
### To uninstall the chart:
```bash
  helm uninstall helium
```

### Local development

```bash
helm template helium charts/helium/ --values charts/helium/values.yaml
```
```bash
helm upgrade --install nginx charts/helium/ --values charts/helium/values.yaml
```
