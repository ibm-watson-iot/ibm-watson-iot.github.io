# IBM Watson IoT Helm Chart Repository

For more information see: https://github.com/helm/helm/blob/master/docs/chart_repository.md

## Updating the Repository

```
$ helm package path/to/chartname -d charts
$ helm repo index . --url https://ibm-watson-iot.github.io/helm/charts/
```


## Using the Repository

```
$ helm repo add wiotp https://ibm-watson-iot.github.io/helm/charts/
$ helm repo list
NAME            URL                                        
wiotp           https://ibm-watson-iot.github.io/helm/charts/
```

### Installation from the Repository

```
$ helm install wiotp/chartname --name=myrelease
```