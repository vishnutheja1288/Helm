# Helm
HelmCharts

minikube Metallb configuration
$kubectl cluster-info
$minikube addons list
$minikube addone enable metallb


Enable metallb >> loadbalancer IP
$minikube ip
$minikube addons metallb configure
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


