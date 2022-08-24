# helm-charts
Helm chart repository
[![Release Charts](https://github.com/CloudClinic-ng/helm-charts/actions/workflows/release.yaml/badge.svg)](https://github.com/CloudClinic-ng/helm-charts/actions/workflows/release.yaml)

## Usage

[Helm](https://helm.sh) must be installed to use the charts.  Please refer to
Helm's [documentation](https://helm.sh/docs) to get started.

Once Helm has been set up correctly, add the repo as follows:
```bash
  helm repo add cloudclinic https://helm.cloudclinic.ng
```

```bash
  helm repo update
```

If you had already added this repo earlier, run `helm repo update` to retrieve
the latest versions of the packages.  You can then run `helm search repo
cloudclinic` to see the charts.

### To install the cloudclinic chart:
```bash
  helm install cloudclinic cloudclinic/cloudclinic
```
### To uninstall the chart:
```bash
  helm uninstall cloudclinic
```

### Local development

```bash
helm template cloudclinic charts/cloudclinic/ --values charts/cloudclinic/values.yaml
```
```bash
helm install cloudclinic charts/cloudclinic/ --values charts/cloudclinic/values.yaml
```
