# tidb-operator
tiDB operator test

kubectl create -f tidb-crd.yaml \
kubectl create ns tidb \
helm install tidb-local . --namespace=tidb \
kubectl create -f tidb-cluster-cr.yaml \
kubectl create secret generic tidb-secret --from-literal=root=admin --namespace=tidb 