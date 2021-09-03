# OpenShift intro


```sh
oc new-project project-intro
oc create configmap nginx-conf --from-file=$(pwd)/nginx-cm/nginx.conf
oc create configmap nginx-html --from-file=$(pwd)/nginx-cm/index.html
oc apply -f ./quote-app.yaml
```