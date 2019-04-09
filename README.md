# pxctl-cheatsheet
Portworx - pxctl cheatsheet

** Check Cluster Status/Health
| Name                                 | Command                                                                          |
|--------------------------------------+----------------------------------------------------------------------------------|
| Run curl test temporarily            | =kubectl run --rm mytest --image=yauritux/busybox-curl -it=                      |
| Run wget test temporarily            | =kubectl run --rm mytest --image=busybox -it=                                    |
| Run nginx deployment with 2 replicas | =kubectl run my-nginx --image=nginx --replicas=2 --port=80=                      |
| Set namespace preference             | =kubectl config set-context $(kubectl config current-context) --namespace=<ns1>= |
| List pods with nodes info            | =kubectl get pod -o wide=                                                        |
