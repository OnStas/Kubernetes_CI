# Kubernetes_CI

commands

mkdir ~/.kube

scp root@kmaster.example.com:efc/kubernates/admin.conf ~/.kube/config

sudo exportfs -v

For Helm

kubectl -n kube-system create serviceaccount tiller

kubectl create clusterrolebinding tiller --clusterrole clusteradmin --serviceaccount=kube-system:tiller

helm init --service -account tiller

kubectl creare -f rbac.yaml -f class.yaml -f deployment.yaml

helm install stable/jenkins


