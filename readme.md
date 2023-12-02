# How to deploy odoo

## Install nfs-subdir-external-provisioner
See https://github.com/Shermine237/NFS-as-PV-provisioner/blob/main/readme.md

## Deploy postgres
```bash
kubectl apply -f  statefulset-postgres.yml
# Wait until postgres is ready
watch kubectl get pod
# Wait ready message in postgres log "database system is ready to accept connections"
kubectl logs postgres-statefulset-0
```

## Deploy Odoo
```bash
kubectl apply -f  statefulset-odoo.yml
```
