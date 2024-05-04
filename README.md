###  helm Installation steps:
```
curl https://raw.githubusercontent.com/helm/helm/master/scripts/get-helm-3 > get_helm.sh
chmod 700 get_helm.sh
./get_helm.sh
```
```
helm version | cut -d + -f 1
```
###  helm Deployment steps:
```
helm create helmchartname
```
```
tree helmchartname
```

or 

```
use ls 
```
```
helm template demohelm 
```
```
helm lint demohelm
```
```
helm install <release_name> <chart_name> [flags]
```
```
helm rollback release_name revsion_number chart_name
```
```
helm upgrade release_name --install chart_name --set image.tag=tag_name
```

```
helm upgrade release_name --install chart_name --set image.tag=tag_name --revision=revision_number
```
```
helm history chart_name --revisions
```
