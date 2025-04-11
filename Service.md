```
**Manually Editing the Service: Alternatively, you can manually edit the service with the following command, which will open the service definition in an edkitor**

[root@masterbm ~]# kubectl get all -n argocd
NAME                                                   READY   STATUS    RESTARTS        AGE
pod/argocd-application-controller-0                    1/1     Running   1 (3h23m ago)   2d
pod/argocd-applicationset-controller-9cbb56dff-9z2tj   1/1     Running   1 (3h23m ago)   2d
pod/argocd-dex-server-74d5d76d7-jhg4n                  1/1     Running   1 (3h23m ago)   2d
pod/argocd-notifications-controller-68459f6cbb-5sb9r   1/1     Running   1 (3h23m ago)   2d
pod/argocd-redis-794f68fb68-lw4cd                      1/1     Running   1 (3h23m ago)   2d
pod/argocd-repo-server-864476c5cf-w6grd                1/1     Running   1 (3h23m ago)   2d
pod/argocd-server-6496dc8859-x5glj                     1/1     Running   1 (3h23m ago)   2d

NAME                                              TYPE        CLUSTER-IP       EXTERNAL-IP   PORT(S)                      AGE
service/argocd-applicationset-controller          ClusterIP   10.98.216.163    <none>        7000/TCP,8080/TCP            2d
service/argocd-dex-server                         ClusterIP   10.102.98.54     <none>        5556/TCP,5557/TCP,5558/TCP   2d
service/argocd-metrics                            ClusterIP   10.96.252.241    <none>        8082/TCP                     2d
service/argocd-notifications-controller-metrics   ClusterIP   10.111.176.60    <none>        9001/TCP                     2d
service/argocd-redis                              ClusterIP   10.101.4.39      <none>        6379/TCP                     2d
service/argocd-repo-server                        ClusterIP   10.101.53.155    <none>        8081/TCP,8084/TCP            2d
service/argocd-server                             ClusterIP   10.110.80.4      <none>        80/TCP,443/TCP               2d
service/argocd-server-metrics                     ClusterIP   10.104.237.222   <none>        8083/TCP                     2d

NAME                                               READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/argocd-applicationset-controller   1/1     1            1           2d
deployment.apps/argocd-dex-server                  1/1     1            1           2d
deployment.apps/argocd-notifications-controller    1/1     1            1           2d
deployment.apps/argocd-redis                       1/1     1            1           2d
deployment.apps/argocd-repo-server                 1/1     1            1           2d
deployment.apps/argocd-server                      1/1     1            1           2d

NAME                                                         DESIRED   CURRENT   READY   AGE
replicaset.apps/argocd-applicationset-controller-9cbb56dff   1         1         1       2d
replicaset.apps/argocd-dex-server-74d5d76d7                  1         1         1       2d
replicaset.apps/argocd-notifications-controller-68459f6cbb   1         1         1       2d
replicaset.apps/argocd-redis-794f68fb68                      1         1         1       2d
replicaset.apps/argocd-repo-server-864476c5cf                1         1         1       2d
replicaset.apps/argocd-server-6496dc8859                     1         1         1       2d

NAME                                             READY   AGE
statefulset.apps/argocd-application-controller   1/1     2d
[root@masterbm ~]# kubectl get pods -n argocd
NAME                                               READY   STATUS    RESTARTS        AGE
argocd-application-controller-0                    1/1     Running   1 (3h23m ago)   2d
argocd-applicationset-controller-9cbb56dff-9z2tj   1/1     Running   1 (3h23m ago)   2d
argocd-dex-server-74d5d76d7-jhg4n                  1/1     Running   1 (3h23m ago)   2d
argocd-notifications-controller-68459f6cbb-5sb9r   1/1     Running   1 (3h23m ago)   2d
argocd-redis-794f68fb68-lw4cd                      1/1     Running   1 (3h23m ago)   2d
argocd-repo-server-864476c5cf-w6grd                1/1     Running   1 (3h23m ago)   2d
argocd-server-6496dc8859-x5glj                     1/1     Running   1 (3h23m ago)   2d
[root@masterbm ~]# kubectl get svc -n argocd
NAME                                      TYPE        CLUSTER-IP       EXTERNAL-IP   PORT(S)                      AGE
argocd-applicationset-controller          ClusterIP   10.98.216.163    <none>        7000/TCP,8080/TCP            2d
argocd-dex-server                         ClusterIP   10.102.98.54     <none>        5556/TCP,5557/TCP,5558/TCP   2d
argocd-metrics                            ClusterIP   10.96.252.241    <none>        8082/TCP                     2d
argocd-notifications-controller-metrics   ClusterIP   10.111.176.60    <none>        9001/TCP                     2d
argocd-redis                              ClusterIP   10.101.4.39      <none>        6379/TCP                     2d
argocd-repo-server                        ClusterIP   10.101.53.155    <none>        8081/TCP,8084/TCP            2d
argocd-server                             ClusterIP   10.110.80.4      <none>        80/TCP,443/TCP               2d
argocd-server-metrics                     ClusterIP   10.104.237.222   <none>        8083/TCP                     2d
[root@masterbm ~]# kubectl describe svc argocd-server -n argocd
Name:                     argocd-server
Namespace:                argocd
Labels:                   app.kubernetes.io/component=server
                          app.kubernetes.io/name=argocd-server
                          app.kubernetes.io/part-of=argocd
Annotations:              <none>
Selector:                 app.kubernetes.io/name=argocd-server
Type:                     ClusterIP
IP Family Policy:         SingleStack
IP Families:              IPv4
IP:                       10.110.80.4
IPs:                      10.110.80.4
Port:                     http  80/TCP
TargetPort:               8080/TCP
Endpoints:                172.16.169.72:8080
Port:                     https  443/TCP
TargetPort:               8080/TCP
Endpoints:                172.16.169.72:8080
Session Affinity:         None
Internal Traffic Policy:  Cluster
Events:                   <none>
[root@masterbm ~]# kubectl get pods -o wide -n argocd
NAME                                               READY   STATUS    RESTARTS        AGE   IP              NODE          NOMINATED NODE   READINESS GATES
argocd-application-controller-0                    1/1     Running   1 (3h24m ago)   2d    172.16.169.69   workerbm-02   <none>           <none>
argocd-applicationset-controller-9cbb56dff-9z2tj   1/1     Running   1 (3h24m ago)   2d    172.16.169.71   workerbm-02   <none>           <none>
argocd-dex-server-74d5d76d7-jhg4n                  1/1     Running   1 (3h24m ago)   2d    172.16.170.5    workerbm-01   <none>           <none>
argocd-notifications-controller-68459f6cbb-5sb9r   1/1     Running   1 (3h24m ago)   2d    172.16.169.70   workerbm-02   <none>           <none>
argocd-redis-794f68fb68-lw4cd                      1/1     Running   1 (3h24m ago)   2d    172.16.170.6    workerbm-01   <none>           <none>
argocd-repo-server-864476c5cf-w6grd                1/1     Running   1 (3h24m ago)   2d    172.16.170.4    workerbm-01   <none>           <none>
argocd-server-6496dc8859-x5glj                     1/1     Running   1 (3h24m ago)   2d    172.16.169.72   workerbm-02   <none>           <none>
[root@masterbm ~]# kubectl get endpoints -n argocd
NAME                                      ENDPOINTS                                               AGE
argocd-applicationset-controller          172.16.169.71:8080,172.16.169.71:7000                   2d
argocd-dex-server                         172.16.170.5:5558,172.16.170.5:5557,172.16.170.5:5556   2d
argocd-metrics                            172.16.169.69:8082                                      2d
argocd-notifications-controller-metrics   172.16.169.70:9001                                      2d
argocd-redis                              172.16.170.6:6379                                       2d
argocd-repo-server                        172.16.170.4:8084,172.16.170.4:8081                     2d
argocd-server                             172.16.169.72:8080,172.16.169.72:8080                   2d
argocd-server-metrics                     172.16.169.72:8083                                      2d
[root@masterbm ~]# kubectl get svc -n argocd
NAME                                      TYPE        CLUSTER-IP       EXTERNAL-IP   PORT(S)                      AGE
argocd-applicationset-controller          ClusterIP   10.98.216.163    <none>        7000/TCP,8080/TCP            2d
argocd-dex-server                         ClusterIP   10.102.98.54     <none>        5556/TCP,5557/TCP,5558/TCP   2d
argocd-metrics                            ClusterIP   10.96.252.241    <none>        8082/TCP                     2d
argocd-notifications-controller-metrics   ClusterIP   10.111.176.60    <none>        9001/TCP                     2d
argocd-redis                              ClusterIP   10.101.4.39      <none>        6379/TCP                     2d
argocd-repo-server                        ClusterIP   10.101.53.155    <none>        8081/TCP,8084/TCP            2d
argocd-server                             ClusterIP   10.110.80.4      <none>        80/TCP,443/TCP               2d
argocd-server-metrics                     ClusterIP   10.104.237.222   <none>        8083/TCP                     2d
[root@masterbm ~]# kubectl edit argocd-server -n argocd
error: the server doesn't have a resource type "argocd-server"
[root@masterbm ~]# kubectl edit svc argocd-server -n argocd
service/argocd-server edited
[root@masterbm ~]# kubectl get svc -n argocd
NAME                                      TYPE        CLUSTER-IP       EXTERNAL-IP   PORT(S)                      AGE
argocd-applicationset-controller          ClusterIP   10.98.216.163    <none>        7000/TCP,8080/TCP            2d
argocd-dex-server                         ClusterIP   10.102.98.54     <none>        5556/TCP,5557/TCP,5558/TCP   2d
argocd-metrics                            ClusterIP   10.96.252.241    <none>        8082/TCP                     2d
argocd-notifications-controller-metrics   ClusterIP   10.111.176.60    <none>        9001/TCP                     2d
argocd-redis                              ClusterIP   10.101.4.39      <none>        6379/TCP                     2d
argocd-repo-server                        ClusterIP   10.101.53.155    <none>        8081/TCP,8084/TCP            2d
argocd-server                             NodePort    10.110.80.4      <none>        80:32598/TCP,443:32193/TCP   2d
argocd-server-metrics                     ClusterIP   10.104.237.222   <none>        8083/TCP                     2d
[root@masterbm ~]# kubectl get endpoints -n argocd
NAME                                      ENDPOINTS                                               AGE
argocd-applicationset-controller          172.16.169.71:8080,172.16.169.71:7000                   2d
argocd-dex-server                         172.16.170.5:5558,172.16.170.5:5557,172.16.170.5:5556   2d
argocd-metrics                            172.16.169.69:8082                                      2d
argocd-notifications-controller-metrics   172.16.169.70:9001                                      2d
argocd-redis                              172.16.170.6:6379                                       2d
argocd-repo-server                        172.16.170.4:8084,172.16.170.4:8081                     2d
argocd-server                             172.16.169.72:8080,172.16.169.72:8080                   2d
argocd-server-metrics                     172.16.169.72:8083                                      2d
[root@masterbm ~]# kubectl describe svc argocd-server -n argocd
Name:                     argocd-server
Namespace:                argocd
Labels:                   app.kubernetes.io/component=server
                          app.kubernetes.io/name=argocd-server
                          app.kubernetes.io/part-of=argocd
Annotations:              <none>
Selector:                 app.kubernetes.io/name=argocd-server
Type:                     NodePort
IP Family Policy:         SingleStack
IP Families:              IPv4
IP:                       10.110.80.4
IPs:                      10.110.80.4
Port:                     http  80/TCP
TargetPort:               8080/TCP
NodePort:                 http  32598/TCP
Endpoints:                172.16.169.72:8080
Port:                     https  443/TCP
TargetPort:               8080/TCP
NodePort:                 https  32193/TCP
Endpoints:                172.16.169.72:8080
Session Affinity:         None
External Traffic Policy:  Cluster
Internal Traffic Policy:  Cluster
Events:                   <none>
[root@masterbm ~]#
```

```
[root@masterbm ~]# ip -br a
lo               UNKNOWN        127.0.0.1/8 ::1/128
enp1s0           UP             192.168.29.150/24
cali1f3a91feb4d@if2 UP             fe80::ecee:eeff:feee:eeee/64
cali0860c8522bc@if2 UP             fe80::ecee:eeff:feee:eeee/64
cali91dc23635c3@if2 UP             fe80::ecee:eeff:feee:eeee/64
tunl0@NONE       UNKNOWN        172.16.149.128/32
[root@masterbm ~]#
[root@masterbm ~]# argocd admin initial-password -n argocd
n7V0CabdjgIRu31T

 This password must be only used for first time login. We strongly recommend you update the password using `argocd account update-password`.
[root@masterbm ~]#


```


![Image Alt](https://github.com/ubuntomathur/ArgoCD/blob/main/argocd.jpg)

now you can login admin/n7V0CabdjgIRu31T














```



[root@masterbm ~]#  argocd admin initial-password -n argocd
n7V0CabdjgIRu31T

 This password must be only used for first time login. We strongly recommend you update the password using `argocd account update-password`.
[root@masterbm ~]# ip -br a
lo               UNKNOWN        127.0.0.1/8 ::1/128
enp1s0           UP             192.168.29.150/24
cali1f3a91feb4d@if2 UP             fe80::ecee:eeff:feee:eeee/64
cali0860c8522bc@if2 UP             fe80::ecee:eeff:feee:eeee/64
cali91dc23635c3@if2 UP             fe80::ecee:eeff:feee:eeee/64
tunl0@NONE       UNKNOWN        172.16.149.128/32
[root@masterbm ~]# kubectl get svc -n agrocd
No resources found in agrocd namespace.
[root@masterbm ~]# kubectl get svc -n argocd
NAME                                      TYPE        CLUSTER-IP       EXTERNAL-IP   PORT(S)                      AGE
argocd-applicationset-controller          ClusterIP   10.98.216.163    <none>        7000/TCP,8080/TCP            2d2h
argocd-dex-server                         ClusterIP   10.102.98.54     <none>        5556/TCP,5557/TCP,5558/TCP   2d2h
argocd-metrics                            ClusterIP   10.96.252.241    <none>        8082/TCP                     2d2h
argocd-notifications-controller-metrics   ClusterIP   10.111.176.60    <none>        9001/TCP                     2d2h
argocd-redis                              ClusterIP   10.101.4.39      <none>        6379/TCP                     2d2h
argocd-repo-server                        ClusterIP   10.101.53.155    <none>        8081/TCP,8084/TCP            2d2h
argocd-server                             NodePort    10.110.80.4      <none>        80:32598/TCP,443:32193/TCP   2d2h
argocd-server-metrics                     ClusterIP   10.104.237.222   <none>        8083/TCP                     2d2h
[root@masterbm ~]# argocd login  192.168.29.15:32598
FATA[0006] dial tcp 192.168.29.15:32598: connect: no route to host
[root@masterbm ~]# kubectl describe svc argocd-server -n argocd
Name:                     argocd-server
Namespace:                argocd
Labels:                   app.kubernetes.io/component=server
                          app.kubernetes.io/name=argocd-server
                          app.kubernetes.io/part-of=argocd
Annotations:              <none>
Selector:                 app.kubernetes.io/name=argocd-server
Type:                     NodePort
IP Family Policy:         SingleStack
IP Families:              IPv4
IP:                       10.110.80.4
IPs:                      10.110.80.4
Port:                     http  80/TCP
TargetPort:               8080/TCP
NodePort:                 http  32598/TCP
Endpoints:                172.16.169.72:8080
Port:                     https  443/TCP
TargetPort:               8080/TCP
NodePort:                 https  32193/TCP
Endpoints:                172.16.169.72:8080
Session Affinity:         None
External Traffic Policy:  Cluster
Internal Traffic Policy:  Cluster
Events:                   <none>
[root@masterbm ~]# cat /etc/hosts
127.0.0.1   localhost localhost.localdomain localhost4 localhost4.localdomain4
::1         localhost localhost.localdomain localhost6 localhost6.localdomain6
[root@masterbm ~]# admin login localhost:32598
-bash: admin: command not found
[root@masterbm ~]# argocd  login localhost:32598
WARNING: server certificate had error: tls: failed to verify certificate: x509: certificate signed by unknown authority. Proceed insecurely (y/n)? y
Username: admin
Password:
'admin:login' logged in successfully
Context 'localhost:32598' updated
[root@masterbm ~]#
```
