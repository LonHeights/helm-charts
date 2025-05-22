# helm-charts
Helm chart repository  
[![Release Charts](https://github.com/CloudClinic-ng/helm-charts/actions/workflows/release.yaml/badge.svg)](https://github.com/CloudClinic-ng/helm-charts/actions/workflows/release.yaml)

## Usage

[Helm](https://helm.sh) must be installed to use the charts.  Please refer to
Helm's [documentation](https://helm.sh/docs) to get started.

Once Helm has been set up correctly, add the repo as follows:
```bash
  helm repo add loh https://helm.cloudclinic.ng
```

```bash
  helm repo update
```

If you had already added this repo earlier, run `helm repo update` to retrieve
the latest versions of the packages.  You can then run `helm search repo
cloudclinic` to see the charts.

### To install the cloudclinic chart:
```bash
  helm install cloudclinic loh/cloudclinic
```

### To install the limestone chart:
```bash
  helm install limestone loh/limestone
```
### To uninstall the chart:
```bash
  helm uninstall cloudclinic
```
```bash
  helm uninstall limestone
```

### Local development

```bash
helm template cloudclinic charts/cloudclinic/ --values charts/cloudclinic/values.yaml
```
```bash
helm upgrade --install nginx charts/cloudclinic/ --values charts/cloudclinic/values.yaml
```

