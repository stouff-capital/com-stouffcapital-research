# https://research.stouffcapital.com

## Deployment

1. `kubectl create -n websites secret generic research --from-literal=mysql-password=<password>`
1. `kubectl create -n websites configmap uploads-ini --from-file=uploads.ini`
1. `kubectl create -f wordpress-db-pvc.yaml`
1. `kubectl create -f wordpress-pvc.yaml`
1. `kubectl create -f wordpress-db-mysql.yaml`
1. `kubectl create -f wordpress-frontend.yaml`
