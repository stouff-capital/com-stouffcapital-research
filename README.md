# https://research.stouffcapital.com

## setup

`kubectl create secret generic research --from-literal=mysql-password=<password>`

`kubectl create configmap uploads-ini --from-file=uploads.ini`
