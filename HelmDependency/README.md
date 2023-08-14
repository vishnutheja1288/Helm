

install deplencies

$ helm dependecny update HelmDependency/
-- it created two folders 'Charts' and 'template'.
-- in charts directory it's downloaded the dependencies

$ helm install test HelmDependency/

$ kubectl get pods

$ helm install test helm-dependency-example --set mysql.enabled=false

$