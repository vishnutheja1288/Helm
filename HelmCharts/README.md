# Helm
HelmCharts

minikube Metallb configuration
$kubectl cluster-info
$minikube addons list
$minikube addone enable metallb


Enable metallb >> loadbalancer IP
$minikube ip
$minikube addons configure metallb
    loadbalancer start Ip:
    loadbalancer end IP:

Treafik install using helm

https://doc.treafik.io/treafik/getting-started/install-traefik/#use-the-helm-chart

$helm repo add traefik https://helm.traefik.io/traefik
$helm repo update
$kubectl create namespace traefik-system
$kubens traefik-system
$helm install traefik traefik/traefik -n traefik-system
$helm statu traefik
$kubectl get po,svc
$

Deploy the application and Skooner dashboard
$kubectl create -f kubectl-app-deployment/

---------------------------------------------
create template
$ helm crate <template name>

$ helm dependency list <folder-name>

$ helm dependency update <folder-name>

$ helm install <any-name> <folder-name>


CHART MUSEUM
---------------

$ chartmuseum --debug --port=8080 --storage="local" --storage-local-rootdir="./chartstorage"

$ helm package helmChart1/

$ curl --data-binay '@mychart-0.1.0.tgz' http://<minikubeip>:8080/api/charts


-------------------------------------------------------------------------------------------------

Dependencies

