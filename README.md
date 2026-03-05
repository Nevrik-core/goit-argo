MacBookAir:hw7 ozzy$ kubectl get pods -n infra-tools
kubectl get svc -n infra-toolsNAME READY STATUS RESTARTS AGE
argocd-application-controller-0 1/1 Running 0 6m1s
argocd-applicationset-controller-64c86665c9-ls8vq 1/1 Running 0 6m1s
argocd-redis-74f7d94755-kzzcj 1/1 Running 0 6m1s
argocd-repo-server-5ddc76c8c9-qlxhv 1/1 Running 0 6m1s
argocd-server-574ccd889c-vjs4z 1/1 Running 0 6m1s
MacBookAir:hw7 ozzy$ kubectl get svc -n infra-tools
NAME TYPE CLUSTER-IP EXTERNAL-IP PORT(S) AGE
argocd-applicationset-controller ClusterIP 172.20.155.55 <none> 7000/TCP 6m4s
argocd-redis ClusterIP 172.20.29.67 <none> 6379/TCP 6m3s
argocd-repo-server ClusterIP 172.20.31.236 <none> 8081/TCP 6m4s
argocd-server ClusterIP 172.20.120.155 <none> 80/TCP,443/TCP 6m4s
MacBookAir:hw7 ozzy$

NAME SYNC STATUS HEALTH STATUS
goit-argo Synced Healthy
mlflow Synced Healthy
MacBookAir:hw7 ozzy$
