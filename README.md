### helm-chart
- go-chart
- java-chart
- nginx-chart

```
helm upgrade --dry-run --debug  --install --force  --timeout 180s --wait --kubeconfig /root/.kube/config \
--set namespace=default \
--set replicaCount=2 \
nginx ./prodchart 

helm upgrade  --install --force  --timeout 180s --wait --kubeconfig /root/.kube/config \
--set namespace=default \
--set replicaCount=8 \
nginx ./prodchart 

```
