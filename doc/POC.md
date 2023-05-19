All necessary settings (cluster, namespace, installation of ArgoSD) have already been completed.

To access the ArgoCD GUI, you need to configure the port with the following command:
kubectl port-forward svc/argocd-server -n argocd 8080:443

After that you need to go to this link in browser:
https://safordog-super-duper-guide-w9pqqxr444whvjgx-8080.preview.app.github.dev/
FYI: you need to use https.

Please use the credentials:
log: admin
psw: cQVB8EyneyBHd3V4