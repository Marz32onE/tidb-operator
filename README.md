# tidb-operator
tiDB operator test

kubectl create -f tidb-crd.yaml
kubectl create ns tidb
helm install tidb-local . --namespace=tidb
kubectl create -f tidb-cluster-cr.yaml 