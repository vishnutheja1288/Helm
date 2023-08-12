

helm Chart2

$ helm dependency list helmChart2/

$ helm dependency update helmchart2/

$ helm install test helmchart2/

$ helm upgrade test helmChart2/

$ helm list

$ helm history test 

Rollback to previous

$ helm rollback test (or)
  helm rollback <release-name> <revision-number>


helm store the each release information in form of secrets
$ kubectl get secrets -n <namespace>

