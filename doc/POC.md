All necessary settings (cluster, namespace, installation of ArgoSD) have already been completed.<br />

To access the ArgoCD GUI, you need to configure the port with the following command:<br />
kubectl port-forward svc/argocd-server -n argocd 8080:443

After that you need to go to this link in browser:<br />
https://safordog-super-duper-guide-w9pqqxr444whvjgx-8080.preview.app.github.dev/<br />
_FYI: you need to use https._

Please use the credentials:<br />
log: admin<br />
psw: cQVB8EyneyBHd3V4