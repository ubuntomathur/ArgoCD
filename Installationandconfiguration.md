```bash
[root@masterbm ~]# kubectl get nodes
NAME          STATUS   ROLES           AGE     VERSION
masterbm      Ready    control-plane   3d17h   v1.31.7
workerbm-01   Ready    <none>          3d17h   v1.31.7
workerbm-02   Ready    <none>          3d17h   v1.31.7

```
```bash
[root@masterbm ~]# kubectl get pods -A
NAMESPACE     NAME                                      READY   STATUS                       RESTARTS      AGE
kube-system   calico-kube-controllers-b8d8894fb-mhg58   0/1     Unknown                      0             3d17h
kube-system   calico-node-4qs8h                         0/1     Unknown                      0             3d17h
kube-system   calico-node-nd7k8                         0/1     Unknown                      0             3d17h
kube-system   calico-node-pj78q                         0/1     Unknown                      0             3d17h
kube-system   coredns-7c65d6cfc9-q8dq9                  0/1     Unknown                      0             3d17h
kube-system   coredns-7c65d6cfc9-twqrd                  0/1     Unknown                      0             3d17h
kube-system   etcd-masterbm                             1/1     Running                      1 (51s ago)   3d17h
kube-system   kube-apiserver-masterbm                   1/1     Running                      1 (51s ago)   3d17h
kube-system   kube-controller-manager-masterbm          1/1     Running                      1 (51s ago)   3d17h
kube-system   kube-proxy-9vhks                          1/1     Running                      1 (51s ago)   3d17h
kube-system   kube-proxy-h4rbt                          1/1     Running                      1 (51s ago)   3d17h
kube-system   kube-proxy-jznhh                          0/1     CreateContainerConfigError   0             3d17h
kube-system   kube-scheduler-masterbm                   1/1     Running                      1 (51s ago)   3d17h
[root@masterbm ~]# kubectl get pods -A
NAMESPACE     NAME                                      READY   STATUS                       RESTARTS      AGE
kube-system   calico-kube-controllers-b8d8894fb-mhg58   0/1     Unknown                      0             3d17h
kube-system   calico-node-4qs8h                         0/1     Unknown                      0             3d17h
kube-system   calico-node-nd7k8                         0/1     Unknown                      0             3d17h
kube-system   calico-node-pj78q                         0/1     Unknown                      0             3d17h
kube-system   coredns-7c65d6cfc9-q8dq9                  0/1     Unknown                      0             3d17h
kube-system   coredns-7c65d6cfc9-twqrd                  0/1     Unknown                      0             3d17h
kube-system   etcd-masterbm                             1/1     Running                      1 (52s ago)   3d17h
kube-system   kube-apiserver-masterbm                   1/1     Running                      1 (52s ago)   3d17h
kube-system   kube-controller-manager-masterbm          1/1     Running                      1 (52s ago)   3d17h
kube-system   kube-proxy-9vhks                          1/1     Running                      1 (52s ago)   3d17h
kube-system   kube-proxy-h4rbt                          1/1     Running                      1 (52s ago)   3d17h
kube-system   kube-proxy-jznhh                          0/1     CreateContainerConfigError   0             3d17h
kube-system   kube-scheduler-masterbm                   1/1     Running                      1 (52s ago)   3d17h
[root@masterbm ~]# kubectl get pods -A
NAMESPACE     NAME                                      READY   STATUS                       RESTARTS      AGE
kube-system   calico-kube-controllers-b8d8894fb-mhg58   0/1     Unknown                      0             3d17h
kube-system   calico-node-4qs8h                         0/1     Unknown                      0             3d17h
kube-system   calico-node-nd7k8                         0/1     Unknown                      0             3d17h
kube-system   calico-node-pj78q                         0/1     Unknown                      0             3d17h
kube-system   coredns-7c65d6cfc9-q8dq9                  0/1     Unknown                      0             3d17h
kube-system   coredns-7c65d6cfc9-twqrd                  0/1     Unknown                      0             3d17h
kube-system   etcd-masterbm                             1/1     Running                      1 (53s ago)   3d17h
kube-system   kube-apiserver-masterbm                   1/1     Running                      1 (53s ago)   3d17h
kube-system   kube-controller-manager-masterbm          1/1     Running                      1 (53s ago)   3d17h
kube-system   kube-proxy-9vhks                          1/1     Running                      1 (53s ago)   3d17h
kube-system   kube-proxy-h4rbt                          1/1     Running                      1 (53s ago)   3d17h
kube-system   kube-proxy-jznhh                          0/1     CreateContainerConfigError   0             3d17h
kube-system   kube-scheduler-masterbm                   1/1     Running                      1 (53s ago)   3d17h
[root@masterbm ~]# kubectl get pods -A
NAMESPACE     NAME                                      READY   STATUS                       RESTARTS      AGE
kube-system   calico-kube-controllers-b8d8894fb-mhg58   0/1     Unknown                      0             3d17h
kube-system   calico-node-4qs8h                         0/1     Unknown                      0             3d17h
kube-system   calico-node-nd7k8                         0/1     Unknown                      0             3d17h
kube-system   calico-node-pj78q                         0/1     Unknown                      0             3d17h
kube-system   coredns-7c65d6cfc9-q8dq9                  0/1     Unknown                      0             3d17h
kube-system   coredns-7c65d6cfc9-twqrd                  0/1     Unknown                      0             3d17h
kube-system   etcd-masterbm                             1/1     Running                      1 (54s ago)   3d17h
kube-system   kube-apiserver-masterbm                   1/1     Running                      1 (54s ago)   3d17h
kube-system   kube-controller-manager-masterbm          1/1     Running                      1 (54s ago)   3d17h
kube-system   kube-proxy-9vhks                          1/1     Running                      1 (54s ago)   3d17h
kube-system   kube-proxy-h4rbt                          1/1     Running                      1 (54s ago)   3d17h
kube-system   kube-proxy-jznhh                          0/1     CreateContainerConfigError   0             3d17h
kube-system   kube-scheduler-masterbm                   1/1     Running                      1 (54s ago)   3d17h
[root@masterbm ~]# kubectl get pods -A
NAMESPACE     NAME                                      READY   STATUS                       RESTARTS      AGE
kube-system   calico-kube-controllers-b8d8894fb-mhg58   0/1     Running                      1 (56s ago)   3d17h
kube-system   calico-node-4qs8h                         0/1     Unknown                      0             3d17h
kube-system   calico-node-nd7k8                         0/1     Unknown                      0             3d17h
kube-system   calico-node-pj78q                         0/1     Unknown                      0             3d17h
kube-system   coredns-7c65d6cfc9-q8dq9                  0/1     Unknown                      0             3d17h
kube-system   coredns-7c65d6cfc9-twqrd                  0/1     Unknown                      0             3d17h
kube-system   etcd-masterbm                             1/1     Running                      1 (56s ago)   3d17h
kube-system   kube-apiserver-masterbm                   1/1     Running                      1 (56s ago)   3d17h
kube-system   kube-controller-manager-masterbm          1/1     Running                      1 (56s ago)   3d17h
kube-system   kube-proxy-9vhks                          1/1     Running                      1 (56s ago)   3d17h
kube-system   kube-proxy-h4rbt                          1/1     Running                      1 (56s ago)   3d17h
kube-system   kube-proxy-jznhh                          0/1     CreateContainerConfigError   0             3d17h
kube-system   kube-scheduler-masterbm                   1/1     Running                      1 (56s ago)   3d17h
[root@masterbm ~]# kubectl get pods -A
NAMESPACE     NAME                                      READY   STATUS                       RESTARTS      AGE
kube-system   calico-kube-controllers-b8d8894fb-mhg58   0/1     Running                      1 (56s ago)   3d17h
kube-system   calico-node-4qs8h                         0/1     Unknown                      0             3d17h
kube-system   calico-node-nd7k8                         0/1     Unknown                      0             3d17h
kube-system   calico-node-pj78q                         0/1     Unknown                      0             3d17h
kube-system   coredns-7c65d6cfc9-q8dq9                  0/1     Unknown                      0             3d17h
kube-system   coredns-7c65d6cfc9-twqrd                  0/1     Unknown                      0             3d17h
kube-system   etcd-masterbm                             1/1     Running                      1 (56s ago)   3d17h
kube-system   kube-apiserver-masterbm                   1/1     Running                      1 (56s ago)   3d17h
kube-system   kube-controller-manager-masterbm          1/1     Running                      1 (56s ago)   3d17h
kube-system   kube-proxy-9vhks                          1/1     Running                      1 (56s ago)   3d17h
kube-system   kube-proxy-h4rbt                          1/1     Running                      1 (56s ago)   3d17h
kube-system   kube-proxy-jznhh                          0/1     CreateContainerConfigError   0             3d17h
kube-system   kube-scheduler-masterbm                   1/1     Running                      1 (56s ago)   3d17h
[root@masterbm ~]# kubectl get pods -A
NAMESPACE     NAME                                      READY   STATUS                       RESTARTS      AGE
kube-system   calico-kube-controllers-b8d8894fb-mhg58   0/1     Running                      1 (57s ago)   3d17h
kube-system   calico-node-4qs8h                         0/1     Unknown                      0             3d17h
kube-system   calico-node-nd7k8                         0/1     Unknown                      0             3d17h
kube-system   calico-node-pj78q                         0/1     Unknown                      0             3d17h
kube-system   coredns-7c65d6cfc9-q8dq9                  0/1     Unknown                      0             3d17h
kube-system   coredns-7c65d6cfc9-twqrd                  0/1     Unknown                      0             3d17h
kube-system   etcd-masterbm                             1/1     Running                      1 (57s ago)   3d17h
kube-system   kube-apiserver-masterbm                   1/1     Running                      1 (57s ago)   3d17h
kube-system   kube-controller-manager-masterbm          1/1     Running                      1 (57s ago)   3d17h
kube-system   kube-proxy-9vhks                          1/1     Running                      1 (57s ago)   3d17h
kube-system   kube-proxy-h4rbt                          1/1     Running                      1 (57s ago)   3d17h
kube-system   kube-proxy-jznhh                          0/1     CreateContainerConfigError   0             3d17h
kube-system   kube-scheduler-masterbm                   1/1     Running                      1 (57s ago)   3d17h
[root@masterbm ~]# kubectl get pods -A
NAMESPACE     NAME                                      READY   STATUS                       RESTARTS      AGE
kube-system   calico-kube-controllers-b8d8894fb-mhg58   0/1     Running                      1 (58s ago)   3d17h
kube-system   calico-node-4qs8h                         0/1     Unknown                      0             3d17h
kube-system   calico-node-nd7k8                         0/1     Unknown                      0             3d17h
kube-system   calico-node-pj78q                         0/1     Unknown                      0             3d17h
kube-system   coredns-7c65d6cfc9-q8dq9                  0/1     Unknown                      0             3d17h
kube-system   coredns-7c65d6cfc9-twqrd                  0/1     Unknown                      0             3d17h
kube-system   etcd-masterbm                             1/1     Running                      1 (58s ago)   3d17h
kube-system   kube-apiserver-masterbm                   1/1     Running                      1 (58s ago)   3d17h
kube-system   kube-controller-manager-masterbm          1/1     Running                      1 (58s ago)   3d17h
kube-system   kube-proxy-9vhks                          1/1     Running                      1 (58s ago)   3d17h
kube-system   kube-proxy-h4rbt                          1/1     Running                      1 (58s ago)   3d17h
kube-system   kube-proxy-jznhh                          0/1     CreateContainerConfigError   0             3d17h
kube-system   kube-scheduler-masterbm                   1/1     Running                      1 (58s ago)   3d17h
[root@masterbm ~]# kubectl get pods -A
NAMESPACE     NAME                                      READY   STATUS                       RESTARTS      AGE
kube-system   calico-kube-controllers-b8d8894fb-mhg58   0/1     Running                      1 (59s ago)   3d17h
kube-system   calico-node-4qs8h                         0/1     Unknown                      0             3d17h
kube-system   calico-node-nd7k8                         0/1     Unknown                      0             3d17h
kube-system   calico-node-pj78q                         0/1     Unknown                      0             3d17h
kube-system   coredns-7c65d6cfc9-q8dq9                  0/1     Unknown                      0             3d17h
kube-system   coredns-7c65d6cfc9-twqrd                  0/1     Unknown                      0             3d17h
kube-system   etcd-masterbm                             1/1     Running                      1 (59s ago)   3d17h
kube-system   kube-apiserver-masterbm                   1/1     Running                      1 (59s ago)   3d17h
kube-system   kube-controller-manager-masterbm          1/1     Running                      1 (59s ago)   3d17h
kube-system   kube-proxy-9vhks                          1/1     Running                      1 (59s ago)   3d17h
kube-system   kube-proxy-h4rbt                          1/1     Running                      1 (59s ago)   3d17h
kube-system   kube-proxy-jznhh                          0/1     CreateContainerConfigError   0             3d17h
kube-system   kube-scheduler-masterbm                   1/1     Running                      1 (59s ago)   3d17h
[root@masterbm ~]# kubectl get pods -A
NAMESPACE     NAME                                      READY   STATUS    RESTARTS      AGE
kube-system   calico-kube-controllers-b8d8894fb-mhg58   0/1     Running   1 (61s ago)   3d17h
kube-system   calico-node-4qs8h                         0/1     Unknown   0             3d17h
kube-system   calico-node-nd7k8                         0/1     Unknown   0             3d17h
kube-system   calico-node-pj78q                         0/1     Unknown   0             3d17h
kube-system   coredns-7c65d6cfc9-q8dq9                  0/1     Unknown   0             3d17h
kube-system   coredns-7c65d6cfc9-twqrd                  0/1     Unknown   0             3d17h
kube-system   etcd-masterbm                             1/1     Running   1 (61s ago)   3d17h
kube-system   kube-apiserver-masterbm                   1/1     Running   1 (61s ago)   3d17h
kube-system   kube-controller-manager-masterbm          1/1     Running   1 (61s ago)   3d17h
kube-system   kube-proxy-9vhks                          1/1     Running   1 (61s ago)   3d17h
kube-system   kube-proxy-h4rbt                          1/1     Running   1 (61s ago)   3d17h
kube-system   kube-proxy-jznhh                          1/1     Running   1 (62s ago)   3d17h
kube-system   kube-scheduler-masterbm                   1/1     Running   1 (61s ago)   3d17h
[root@masterbm ~]# kubectl get pods -A
NAMESPACE     NAME                                      READY   STATUS    RESTARTS      AGE
kube-system   calico-kube-controllers-b8d8894fb-mhg58   0/1     Running   1 (64s ago)   3d17h
kube-system   calico-node-4qs8h                         0/1     Unknown   0             3d17h
kube-system   calico-node-nd7k8                         0/1     Unknown   0             3d17h
kube-system   calico-node-pj78q                         0/1     Unknown   0             3d17h
kube-system   coredns-7c65d6cfc9-q8dq9                  0/1     Unknown   0             3d17h
kube-system   coredns-7c65d6cfc9-twqrd                  0/1     Running   1 (64s ago)   3d17h
kube-system   etcd-masterbm                             1/1     Running   1 (64s ago)   3d17h
kube-system   kube-apiserver-masterbm                   1/1     Running   1 (64s ago)   3d17h
kube-system   kube-controller-manager-masterbm          1/1     Running   1 (64s ago)   3d17h
kube-system   kube-proxy-9vhks                          1/1     Running   1 (64s ago)   3d17h
kube-system   kube-proxy-h4rbt                          1/1     Running   1 (64s ago)   3d17h
kube-system   kube-proxy-jznhh                          1/1     Running   1 (65s ago)   3d17h
kube-system   kube-scheduler-masterbm                   1/1     Running   1 (64s ago)   3d17h
[root@masterbm ~]# kubectl get pods -A
NAMESPACE     NAME                                      READY   STATUS    RESTARTS      AGE
kube-system   calico-kube-controllers-b8d8894fb-mhg58   1/1     Running   1 (45m ago)   3d18h
kube-system   calico-node-4qs8h                         1/1     Running   1 (45m ago)   3d18h
kube-system   calico-node-nd7k8                         1/1     Running   1 (45m ago)   3d18h
kube-system   calico-node-pj78q                         1/1     Running   1 (45m ago)   3d18h
kube-system   coredns-7c65d6cfc9-q8dq9                  1/1     Running   1 (45m ago)   3d18h
kube-system   coredns-7c65d6cfc9-twqrd                  1/1     Running   1 (45m ago)   3d18h
kube-system   etcd-masterbm                             1/1     Running   1 (45m ago)   3d18h
kube-system   kube-apiserver-masterbm                   1/1     Running   1 (45m ago)   3d18h
kube-system   kube-controller-manager-masterbm          1/1     Running   1 (45m ago)   3d18h
kube-system   kube-proxy-9vhks                          1/1     Running   1 (45m ago)   3d18h
kube-system   kube-proxy-h4rbt                          1/1     Running   1 (45m ago)   3d18h
kube-system   kube-proxy-jznhh                          1/1     Running   1 (45m ago)   3d18h
kube-system   kube-scheduler-masterbm                   1/1     Running   1 (45m ago)   3d18h
```

```bash
[root@masterbm ~]# kubectl create namespace argocd
namespace/argocd created
[root@masterbm ~]# kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml
customresourcedefinition.apiextensions.k8s.io/applications.argoproj.io created
customresourcedefinition.apiextensions.k8s.io/applicationsets.argoproj.io created
customresourcedefinition.apiextensions.k8s.io/appprojects.argoproj.io created
serviceaccount/argocd-application-controller created
serviceaccount/argocd-applicationset-controller created
serviceaccount/argocd-dex-server created
serviceaccount/argocd-notifications-controller created
serviceaccount/argocd-redis created
serviceaccount/argocd-repo-server created
serviceaccount/argocd-server created
role.rbac.authorization.k8s.io/argocd-application-controller created
role.rbac.authorization.k8s.io/argocd-applicationset-controller created
role.rbac.authorization.k8s.io/argocd-dex-server created
role.rbac.authorization.k8s.io/argocd-notifications-controller created
role.rbac.authorization.k8s.io/argocd-redis created
role.rbac.authorization.k8s.io/argocd-server created
clusterrole.rbac.authorization.k8s.io/argocd-application-controller created
clusterrole.rbac.authorization.k8s.io/argocd-applicationset-controller created
clusterrole.rbac.authorization.k8s.io/argocd-server created
rolebinding.rbac.authorization.k8s.io/argocd-application-controller created
rolebinding.rbac.authorization.k8s.io/argocd-applicationset-controller created
rolebinding.rbac.authorization.k8s.io/argocd-dex-server created
rolebinding.rbac.authorization.k8s.io/argocd-notifications-controller created
rolebinding.rbac.authorization.k8s.io/argocd-redis created
rolebinding.rbac.authorization.k8s.io/argocd-server created
clusterrolebinding.rbac.authorization.k8s.io/argocd-application-controller created
clusterrolebinding.rbac.authorization.k8s.io/argocd-applicationset-controller created
clusterrolebinding.rbac.authorization.k8s.io/argocd-server created
configmap/argocd-cm created
configmap/argocd-cmd-params-cm created
configmap/argocd-gpg-keys-cm created
configmap/argocd-notifications-cm created
configmap/argocd-rbac-cm created
configmap/argocd-ssh-known-hosts-cm created
configmap/argocd-tls-certs-cm created
secret/argocd-notifications-secret created
secret/argocd-secret created
service/argocd-applicationset-controller created
service/argocd-dex-server created
service/argocd-metrics created
service/argocd-notifications-controller-metrics created
service/argocd-redis created
service/argocd-repo-server created
service/argocd-server created
service/argocd-server-metrics created
deployment.apps/argocd-applicationset-controller created
deployment.apps/argocd-dex-server created
deployment.apps/argocd-notifications-controller created
deployment.apps/argocd-redis created
deployment.apps/argocd-repo-server created
deployment.apps/argocd-server created
statefulset.apps/argocd-application-controller created
networkpolicy.networking.k8s.io/argocd-application-controller-network-policy created
networkpolicy.networking.k8s.io/argocd-applicationset-controller-network-policy created
networkpolicy.networking.k8s.io/argocd-dex-server-network-policy created
networkpolicy.networking.k8s.io/argocd-notifications-controller-network-policy created
networkpolicy.networking.k8s.io/argocd-redis-network-policy created
networkpolicy.networking.k8s.io/argocd-repo-server-network-policy created
networkpolicy.networking.k8s.io/argocd-server-network-policy created

```
```bash
[root@masterbm ~]# kubectl get all --namespace=argocd
NAME                                                   READY   STATUS              RESTARTS   AGE
pod/argocd-application-controller-0                    0/1     ContainerCreating   0          7s
pod/argocd-applicationset-controller-9cbb56dff-9z2tj   0/1     ContainerCreating   0          8s
pod/argocd-dex-server-74d5d76d7-jhg4n                  0/1     Init:0/1            0          8s
pod/argocd-notifications-controller-68459f6cbb-5sb9r   0/1     ContainerCreating   0          8s
pod/argocd-redis-794f68fb68-lw4cd                      0/1     Init:0/1            0          7s
pod/argocd-repo-server-864476c5cf-w6grd                0/1     Init:0/1            0          7s
pod/argocd-server-6496dc8859-x5glj                     0/1     ContainerCreating   0          7s


```
```bash
NAME                                              TYPE        CLUSTER-IP       EXTERNAL-IP   PORT(S)                      AGE
service/argocd-applicationset-controller          ClusterIP   10.98.216.163    <none>        7000/TCP,8080/TCP            8s
service/argocd-dex-server                         ClusterIP   10.102.98.54     <none>        5556/TCP,5557/TCP,5558/TCP   8s
service/argocd-metrics                            ClusterIP   10.96.252.241    <none>        8082/TCP                     8s
service/argocd-notifications-controller-metrics   ClusterIP   10.111.176.60    <none>        9001/TCP                     8s
service/argocd-redis                              ClusterIP   10.101.4.39      <none>        6379/TCP                     8s
service/argocd-repo-server                        ClusterIP   10.101.53.155    <none>        8081/TCP,8084/TCP            8s
service/argocd-server                             ClusterIP   10.110.80.4      <none>        80/TCP,443/TCP               8s
service/argocd-server-metrics                     ClusterIP   10.104.237.222   <none>        8083/TCP                     8s

```bash
NAME                                               READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/argocd-applicationset-controller   0/1     1            0           8s
deployment.apps/argocd-dex-server                  0/1     1            0           8s
deployment.apps/argocd-notifications-controller    0/1     1            0           8s
deployment.apps/argocd-redis                       0/1     1            0           7s
deployment.apps/argocd-repo-server                 0/1     1            0           7s
deployment.apps/argocd-server                      0/1     1            0           7s
```bash
NAME                                                         DESIRED   CURRENT   READY   AGE
replicaset.apps/argocd-applicationset-controller-9cbb56dff   1         1         0       8s
replicaset.apps/argocd-dex-server-74d5d76d7                  1         1         0       8s
replicaset.apps/argocd-notifications-controller-68459f6cbb   1         1         0       8s
replicaset.apps/argocd-redis-794f68fb68                      1         1         0       7s
replicaset.apps/argocd-repo-server-864476c5cf                1         1         0       7s
replicaset.apps/argocd-server-6496dc8859                     1         1         0       7s
```bash
NAME                                             READY   AGE
statefulset.apps/argocd-application-controller   0/1     7s
[root@masterbm ~]# kubectl get all --namespace=argocd
NAME                                                   READY   STATUS              RESTARTS   AGE
pod/argocd-application-controller-0                    0/1     ContainerCreating   0          11s
pod/argocd-applicationset-controller-9cbb56dff-9z2tj   0/1     ContainerCreating   0          12s
pod/argocd-dex-server-74d5d76d7-jhg4n                  0/1     Init:0/1            0          12s
pod/argocd-notifications-controller-68459f6cbb-5sb9r   0/1     ContainerCreating   0          12s
pod/argocd-redis-794f68fb68-lw4cd                      0/1     Init:0/1            0          11s
pod/argocd-repo-server-864476c5cf-w6grd                0/1     Init:0/1            0          11s
pod/argocd-server-6496dc8859-x5glj                     0/1     ContainerCreating   0          11s
```bash
NAME                                              TYPE        CLUSTER-IP       EXTERNAL-IP   PORT(S)                      AGE
service/argocd-applicationset-controller          ClusterIP   10.98.216.163    <none>        7000/TCP,8080/TCP            12s
service/argocd-dex-server                         ClusterIP   10.102.98.54     <none>        5556/TCP,5557/TCP,5558/TCP   12s
service/argocd-metrics                            ClusterIP   10.96.252.241    <none>        8082/TCP                     12s
service/argocd-notifications-controller-metrics   ClusterIP   10.111.176.60    <none>        9001/TCP                     12s
service/argocd-redis                              ClusterIP   10.101.4.39      <none>        6379/TCP                     12s
service/argocd-repo-server                        ClusterIP   10.101.53.155    <none>        8081/TCP,8084/TCP            12s
service/argocd-server                             ClusterIP   10.110.80.4      <none>        80/TCP,443/TCP               12s
service/argocd-server-metrics                     ClusterIP   10.104.237.222   <none>        8083/TCP                     12s
```bash
NAME                                               READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/argocd-applicationset-controller   0/1     1            0           12s
deployment.apps/argocd-dex-server                  0/1     1            0           12s
deployment.apps/argocd-notifications-controller    0/1     1            0           12s
deployment.apps/argocd-redis                       0/1     1            0           11s
deployment.apps/argocd-repo-server                 0/1     1            0           11s
deployment.apps/argocd-server                      0/1     1            0           11s
```bash
NAME                                                         DESIRED   CURRENT   READY   AGE
replicaset.apps/argocd-applicationset-controller-9cbb56dff   1         1         0       12s
replicaset.apps/argocd-dex-server-74d5d76d7                  1         1         0       12s
replicaset.apps/argocd-notifications-controller-68459f6cbb   1         1         0       12s
replicaset.apps/argocd-redis-794f68fb68                      1         1         0       11s
replicaset.apps/argocd-repo-server-864476c5cf                1         1         0       11s
replicaset.apps/argocd-server-6496dc8859                     1         1         0       11s

NAME                                             READY   AGE
statefulset.apps/argocd-application-controller   0/1     11s
[root@masterbm ~]#
[root@masterbm ~]# kubectl get all --namespace=argocd
NAME                                                   READY   STATUS              RESTARTS   AGE
pod/argocd-application-controller-0                    0/1     ContainerCreating   0          12s
pod/argocd-applicationset-controller-9cbb56dff-9z2tj   0/1     ContainerCreating   0          13s
pod/argocd-dex-server-74d5d76d7-jhg4n                  0/1     Init:0/1            0          13s
pod/argocd-notifications-controller-68459f6cbb-5sb9r   0/1     ContainerCreating   0          13s
pod/argocd-redis-794f68fb68-lw4cd                      0/1     Init:0/1            0          12s
pod/argocd-repo-server-864476c5cf-w6grd                0/1     Init:0/1            0          12s
pod/argocd-server-6496dc8859-x5glj                     0/1     ContainerCreating   0          12s

NAME                                              TYPE        CLUSTER-IP       EXTERNAL-IP   PORT(S)                      AGE
service/argocd-applicationset-controller          ClusterIP   10.98.216.163    <none>        7000/TCP,8080/TCP            13s
service/argocd-dex-server                         ClusterIP   10.102.98.54     <none>        5556/TCP,5557/TCP,5558/TCP   13s
service/argocd-metrics                            ClusterIP   10.96.252.241    <none>        8082/TCP                     13s
service/argocd-notifications-controller-metrics   ClusterIP   10.111.176.60    <none>        9001/TCP                     13s
service/argocd-redis                              ClusterIP   10.101.4.39      <none>        6379/TCP                     13s
service/argocd-repo-server                        ClusterIP   10.101.53.155    <none>        8081/TCP,8084/TCP            13s
service/argocd-server                             ClusterIP   10.110.80.4      <none>        80/TCP,443/TCP               13s
service/argocd-server-metrics                     ClusterIP   10.104.237.222   <none>        8083/TCP                     13s

NAME                                               READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/argocd-applicationset-controller   0/1     1            0           13s
deployment.apps/argocd-dex-server                  0/1     1            0           13s
deployment.apps/argocd-notifications-controller    0/1     1            0           13s
deployment.apps/argocd-redis                       0/1     1            0           12s
deployment.apps/argocd-repo-server                 0/1     1            0           12s
deployment.apps/argocd-server                      0/1     1            0           12s
```bash
NAME                                                         DESIRED   CURRENT   READY   AGE
replicaset.apps/argocd-applicationset-controller-9cbb56dff   1         1         0       13s
replicaset.apps/argocd-dex-server-74d5d76d7                  1         1         0       13s
replicaset.apps/argocd-notifications-controller-68459f6cbb   1         1         0       13s
replicaset.apps/argocd-redis-794f68fb68                      1         1         0       12s
replicaset.apps/argocd-repo-server-864476c5cf                1         1         0       12s
replicaset.apps/argocd-server-6496dc8859                     1         1         0       12s
```bash
NAME                                             READY   AGE
statefulset.apps/argocd-application-controller   0/1     12s
[root@masterbm ~]# kubectl get all --namespace=argocd
NAME                                                   READY   STATUS              RESTARTS   AGE
pod/argocd-application-controller-0                    0/1     ContainerCreating   0          13s
pod/argocd-applicationset-controller-9cbb56dff-9z2tj   0/1     ContainerCreating   0          14s
pod/argocd-dex-server-74d5d76d7-jhg4n                  0/1     Init:0/1            0          14s
pod/argocd-notifications-controller-68459f6cbb-5sb9r   0/1     ContainerCreating   0          14s
pod/argocd-redis-794f68fb68-lw4cd                      0/1     Init:0/1            0          13s
pod/argocd-repo-server-864476c5cf-w6grd                0/1     Init:0/1            0          13s
pod/argocd-server-6496dc8859-x5glj                     0/1     ContainerCreating   0          13s
```bash
NAME                                              TYPE        CLUSTER-IP       EXTERNAL-IP   PORT(S)                      AGE
service/argocd-applicationset-controller          ClusterIP   10.98.216.163    <none>        7000/TCP,8080/TCP            14s
service/argocd-dex-server                         ClusterIP   10.102.98.54     <none>        5556/TCP,5557/TCP,5558/TCP   14s
service/argocd-metrics                            ClusterIP   10.96.252.241    <none>        8082/TCP                     14s
service/argocd-notifications-controller-metrics   ClusterIP   10.111.176.60    <none>        9001/TCP                     14s
service/argocd-redis                              ClusterIP   10.101.4.39      <none>        6379/TCP                     14s
service/argocd-repo-server                        ClusterIP   10.101.53.155    <none>        8081/TCP,8084/TCP            14s
service/argocd-server                             ClusterIP   10.110.80.4      <none>        80/TCP,443/TCP               14s
service/argocd-server-metrics                     ClusterIP   10.104.237.222   <none>        8083/TCP                     14s
```bash
NAME                                               READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/argocd-applicationset-controller   0/1     1            0           14s
deployment.apps/argocd-dex-server                  0/1     1            0           14s
deployment.apps/argocd-notifications-controller    0/1     1            0           14s
deployment.apps/argocd-redis                       0/1     1            0           13s
deployment.apps/argocd-repo-server                 0/1     1            0           13s
deployment.apps/argocd-server                      0/1     1            0           13s
```bash
NAME                                                         DESIRED   CURRENT   READY   AGE
replicaset.apps/argocd-applicationset-controller-9cbb56dff   1         1         0       14s
replicaset.apps/argocd-dex-server-74d5d76d7                  1         1         0       14s
replicaset.apps/argocd-notifications-controller-68459f6cbb   1         1         0       14s
replicaset.apps/argocd-redis-794f68fb68                      1         1         0       13s
replicaset.apps/argocd-repo-server-864476c5cf                1         1         0       13s
replicaset.apps/argocd-server-6496dc8859                     1         1         0       13s
```bash
NAME                                             READY   AGE
statefulset.apps/argocd-application-controller   0/1     13s
[root@masterbm ~]# kubectl get all --namespace=argocd
NAME                                                   READY   STATUS              RESTARTS   AGE
pod/argocd-application-controller-0                    0/1     ContainerCreating   0          15s
pod/argocd-applicationset-controller-9cbb56dff-9z2tj   0/1     ContainerCreating   0          16s
pod/argocd-dex-server-74d5d76d7-jhg4n                  0/1     Init:0/1            0          16s
pod/argocd-notifications-controller-68459f6cbb-5sb9r   0/1     ContainerCreating   0          16s
pod/argocd-redis-794f68fb68-lw4cd                      0/1     Init:0/1            0          15s
pod/argocd-repo-server-864476c5cf-w6grd                0/1     Init:0/1            0          15s
pod/argocd-server-6496dc8859-x5glj                     0/1     ContainerCreating   0          15s
```bash
NAME                                              TYPE        CLUSTER-IP       EXTERNAL-IP   PORT(S)                      AGE
service/argocd-applicationset-controller          ClusterIP   10.98.216.163    <none>        7000/TCP,8080/TCP            16s
service/argocd-dex-server                         ClusterIP   10.102.98.54     <none>        5556/TCP,5557/TCP,5558/TCP   16s
service/argocd-metrics                            ClusterIP   10.96.252.241    <none>        8082/TCP                     16s
service/argocd-notifications-controller-metrics   ClusterIP   10.111.176.60    <none>        9001/TCP                     16s
service/argocd-redis                              ClusterIP   10.101.4.39      <none>        6379/TCP                     16s
service/argocd-repo-server                        ClusterIP   10.101.53.155    <none>        8081/TCP,8084/TCP            16s
service/argocd-server                             ClusterIP   10.110.80.4      <none>        80/TCP,443/TCP               16s
service/argocd-server-metrics                     ClusterIP   10.104.237.222   <none>        8083/TCP                     16s

NAME                                               READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/argocd-applicationset-controller   0/1     1            0           16s
deployment.apps/argocd-dex-server                  0/1     1            0           16s
deployment.apps/argocd-notifications-controller    0/1     1            0           16s
deployment.apps/argocd-redis                       0/1     1            0           15s
deployment.apps/argocd-repo-server                 0/1     1            0           15s
deployment.apps/argocd-server                      0/1     1            0           15s

NAME                                                         DESIRED   CURRENT   READY   AGE
replicaset.apps/argocd-applicationset-controller-9cbb56dff   1         1         0       16s
replicaset.apps/argocd-dex-server-74d5d76d7                  1         1         0       16s
replicaset.apps/argocd-notifications-controller-68459f6cbb   1         1         0       16s
replicaset.apps/argocd-redis-794f68fb68                      1         1         0       15s
replicaset.apps/argocd-repo-server-864476c5cf                1         1         0       15s
replicaset.apps/argocd-server-6496dc8859                     1         1         0       15s

NAME                                             READY   AGE
statefulset.apps/argocd-application-controller   0/1     15s
[root@masterbm ~]# kubectl get all --namespace=argocd
NAME                                                   READY   STATUS              RESTARTS   AGE
pod/argocd-application-controller-0                    0/1     ContainerCreating   0          16s
pod/argocd-applicationset-controller-9cbb56dff-9z2tj   0/1     ContainerCreating   0          17s
pod/argocd-dex-server-74d5d76d7-jhg4n                  0/1     Init:0/1            0          17s
pod/argocd-notifications-controller-68459f6cbb-5sb9r   0/1     ContainerCreating   0          17s
pod/argocd-redis-794f68fb68-lw4cd                      0/1     Init:0/1            0          16s
pod/argocd-repo-server-864476c5cf-w6grd                0/1     Init:0/1            0          16s
pod/argocd-server-6496dc8859-x5glj                     0/1     ContainerCreating   0          16s

NAME                                              TYPE        CLUSTER-IP       EXTERNAL-IP   PORT(S)                      AGE
service/argocd-applicationset-controller          ClusterIP   10.98.216.163    <none>        7000/TCP,8080/TCP            17s
service/argocd-dex-server                         ClusterIP   10.102.98.54     <none>        5556/TCP,5557/TCP,5558/TCP   17s
service/argocd-metrics                            ClusterIP   10.96.252.241    <none>        8082/TCP                     17s
service/argocd-notifications-controller-metrics   ClusterIP   10.111.176.60    <none>        9001/TCP                     17s
service/argocd-redis                              ClusterIP   10.101.4.39      <none>        6379/TCP                     17s
service/argocd-repo-server                        ClusterIP   10.101.53.155    <none>        8081/TCP,8084/TCP            17s
service/argocd-server                             ClusterIP   10.110.80.4      <none>        80/TCP,443/TCP               17s
service/argocd-server-metrics                     ClusterIP   10.104.237.222   <none>        8083/TCP                     17s

NAME                                               READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/argocd-applicationset-controller   0/1     1            0           17s
deployment.apps/argocd-dex-server                  0/1     1            0           17s
deployment.apps/argocd-notifications-controller    0/1     1            0           17s
deployment.apps/argocd-redis                       0/1     1            0           16s
deployment.apps/argocd-repo-server                 0/1     1            0           16s
deployment.apps/argocd-server                      0/1     1            0           16s

NAME                                                         DESIRED   CURRENT   READY   AGE
replicaset.apps/argocd-applicationset-controller-9cbb56dff   1         1         0       17s
replicaset.apps/argocd-dex-server-74d5d76d7                  1         1         0       17s
replicaset.apps/argocd-notifications-controller-68459f6cbb   1         1         0       17s
replicaset.apps/argocd-redis-794f68fb68                      1         1         0       16s
replicaset.apps/argocd-repo-server-864476c5cf                1         1         0       16s
replicaset.apps/argocd-server-6496dc8859                     1         1         0       16s

NAME                                             READY   AGE
statefulset.apps/argocd-application-controller   0/1     16s
[root@masterbm ~]# kubectl get all --namespace=argocd
NAME                                                   READY   STATUS              RESTARTS   AGE
pod/argocd-application-controller-0                    0/1     ContainerCreating   0          17s
pod/argocd-applicationset-controller-9cbb56dff-9z2tj   0/1     ContainerCreating   0          18s
pod/argocd-dex-server-74d5d76d7-jhg4n                  0/1     Init:0/1            0          18s
pod/argocd-notifications-controller-68459f6cbb-5sb9r   0/1     ContainerCreating   0          18s
pod/argocd-redis-794f68fb68-lw4cd                      0/1     Init:0/1            0          17s
pod/argocd-repo-server-864476c5cf-w6grd                0/1     Init:0/1            0          17s
pod/argocd-server-6496dc8859-x5glj                     0/1     ContainerCreating   0          17s

NAME                                              TYPE        CLUSTER-IP       EXTERNAL-IP   PORT(S)                      AGE
service/argocd-applicationset-controller          ClusterIP   10.98.216.163    <none>        7000/TCP,8080/TCP            18s
service/argocd-dex-server                         ClusterIP   10.102.98.54     <none>        5556/TCP,5557/TCP,5558/TCP   18s
service/argocd-metrics                            ClusterIP   10.96.252.241    <none>        8082/TCP                     18s
service/argocd-notifications-controller-metrics   ClusterIP   10.111.176.60    <none>        9001/TCP                     18s
service/argocd-redis                              ClusterIP   10.101.4.39      <none>        6379/TCP                     18s
service/argocd-repo-server                        ClusterIP   10.101.53.155    <none>        8081/TCP,8084/TCP            18s
service/argocd-server                             ClusterIP   10.110.80.4      <none>        80/TCP,443/TCP               18s
service/argocd-server-metrics                     ClusterIP   10.104.237.222   <none>        8083/TCP                     18s

NAME                                               READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/argocd-applicationset-controller   0/1     1            0           18s
deployment.apps/argocd-dex-server                  0/1     1            0           18s
deployment.apps/argocd-notifications-controller    0/1     1            0           18s
deployment.apps/argocd-redis                       0/1     1            0           17s
deployment.apps/argocd-repo-server                 0/1     1            0           17s
deployment.apps/argocd-server                      0/1     1            0           17s

NAME                                                         DESIRED   CURRENT   READY   AGE
replicaset.apps/argocd-applicationset-controller-9cbb56dff   1         1         0       18s
replicaset.apps/argocd-dex-server-74d5d76d7                  1         1         0       18s
replicaset.apps/argocd-notifications-controller-68459f6cbb   1         1         0       18s
replicaset.apps/argocd-redis-794f68fb68                      1         1         0       17s
replicaset.apps/argocd-repo-server-864476c5cf                1         1         0       17s
replicaset.apps/argocd-server-6496dc8859                     1         1         0       17s

NAME                                             READY   AGE
statefulset.apps/argocd-application-controller   0/1     17s
[root@masterbm ~]# kubectl get all --namespace=argocd
NAME                                                   READY   STATUS              RESTARTS   AGE
pod/argocd-application-controller-0                    0/1     ContainerCreating   0          19s
pod/argocd-applicationset-controller-9cbb56dff-9z2tj   0/1     ContainerCreating   0          20s
pod/argocd-dex-server-74d5d76d7-jhg4n                  0/1     Init:0/1            0          20s
pod/argocd-notifications-controller-68459f6cbb-5sb9r   0/1     ContainerCreating   0          20s
pod/argocd-redis-794f68fb68-lw4cd                      0/1     Init:0/1            0          19s
pod/argocd-repo-server-864476c5cf-w6grd                0/1     Init:0/1            0          19s
pod/argocd-server-6496dc8859-x5glj                     0/1     ContainerCreating   0          19s

NAME                                              TYPE        CLUSTER-IP       EXTERNAL-IP   PORT(S)                      AGE
service/argocd-applicationset-controller          ClusterIP   10.98.216.163    <none>        7000/TCP,8080/TCP            20s
service/argocd-dex-server                         ClusterIP   10.102.98.54     <none>        5556/TCP,5557/TCP,5558/TCP   20s
service/argocd-metrics                            ClusterIP   10.96.252.241    <none>        8082/TCP                     20s
service/argocd-notifications-controller-metrics   ClusterIP   10.111.176.60    <none>        9001/TCP                     20s
service/argocd-redis                              ClusterIP   10.101.4.39      <none>        6379/TCP                     20s
service/argocd-repo-server                        ClusterIP   10.101.53.155    <none>        8081/TCP,8084/TCP            20s
service/argocd-server                             ClusterIP   10.110.80.4      <none>        80/TCP,443/TCP               20s
service/argocd-server-metrics                     ClusterIP   10.104.237.222   <none>        8083/TCP                     20s

NAME                                               READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/argocd-applicationset-controller   0/1     1            0           20s
deployment.apps/argocd-dex-server                  0/1     1            0           20s
deployment.apps/argocd-notifications-controller    0/1     1            0           20s
deployment.apps/argocd-redis                       0/1     1            0           19s
deployment.apps/argocd-repo-server                 0/1     1            0           19s
deployment.apps/argocd-server                      0/1     1            0           19s

NAME                                                         DESIRED   CURRENT   READY   AGE
replicaset.apps/argocd-applicationset-controller-9cbb56dff   1         1         0       20s
replicaset.apps/argocd-dex-server-74d5d76d7                  1         1         0       20s
replicaset.apps/argocd-notifications-controller-68459f6cbb   1         1         0       20s
replicaset.apps/argocd-redis-794f68fb68                      1         1         0       19s
replicaset.apps/argocd-repo-server-864476c5cf                1         1         0       19s
replicaset.apps/argocd-server-6496dc8859                     1         1         0       19s

NAME                                             READY   AGE
statefulset.apps/argocd-application-controller   0/1     19s
[root@masterbm ~]# kubectl get all --namespace=argocd
NAME                                                   READY   STATUS              RESTARTS   AGE
pod/argocd-application-controller-0                    0/1     ContainerCreating   0          20s
pod/argocd-applicationset-controller-9cbb56dff-9z2tj   0/1     ContainerCreating   0          21s
pod/argocd-dex-server-74d5d76d7-jhg4n                  0/1     Init:0/1            0          21s
pod/argocd-notifications-controller-68459f6cbb-5sb9r   0/1     ContainerCreating   0          21s
pod/argocd-redis-794f68fb68-lw4cd                      0/1     Init:0/1            0          20s
pod/argocd-repo-server-864476c5cf-w6grd                0/1     Init:0/1            0          20s
pod/argocd-server-6496dc8859-x5glj                     0/1     ContainerCreating   0          20s

NAME                                              TYPE        CLUSTER-IP       EXTERNAL-IP   PORT(S)                      AGE
service/argocd-applicationset-controller          ClusterIP   10.98.216.163    <none>        7000/TCP,8080/TCP            21s
service/argocd-dex-server                         ClusterIP   10.102.98.54     <none>        5556/TCP,5557/TCP,5558/TCP   21s
service/argocd-metrics                            ClusterIP   10.96.252.241    <none>        8082/TCP                     21s
service/argocd-notifications-controller-metrics   ClusterIP   10.111.176.60    <none>        9001/TCP                     21s
service/argocd-redis                              ClusterIP   10.101.4.39      <none>        6379/TCP                     21s
service/argocd-repo-server                        ClusterIP   10.101.53.155    <none>        8081/TCP,8084/TCP            21s
service/argocd-server                             ClusterIP   10.110.80.4      <none>        80/TCP,443/TCP               21s
service/argocd-server-metrics                     ClusterIP   10.104.237.222   <none>        8083/TCP                     21s

NAME                                               READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/argocd-applicationset-controller   0/1     1            0           21s
deployment.apps/argocd-dex-server                  0/1     1            0           21s
deployment.apps/argocd-notifications-controller    0/1     1            0           21s
deployment.apps/argocd-redis                       0/1     1            0           20s
deployment.apps/argocd-repo-server                 0/1     1            0           20s
deployment.apps/argocd-server                      0/1     1            0           20s

NAME                                                         DESIRED   CURRENT   READY   AGE
replicaset.apps/argocd-applicationset-controller-9cbb56dff   1         1         0       21s
replicaset.apps/argocd-dex-server-74d5d76d7                  1         1         0       21s
replicaset.apps/argocd-notifications-controller-68459f6cbb   1         1         0       21s
replicaset.apps/argocd-redis-794f68fb68                      1         1         0       20s
replicaset.apps/argocd-repo-server-864476c5cf                1         1         0       20s
replicaset.apps/argocd-server-6496dc8859                     1         1         0       20s

NAME                                             READY   AGE
statefulset.apps/argocd-application-controller   0/1     20s
[root@masterbm ~]# kubectl get all --namespace=argocd
NAME                                                   READY   STATUS              RESTARTS   AGE
pod/argocd-application-controller-0                    0/1     ContainerCreating   0          25s
pod/argocd-applicationset-controller-9cbb56dff-9z2tj   0/1     ContainerCreating   0          26s
pod/argocd-dex-server-74d5d76d7-jhg4n                  0/1     Init:0/1            0          26s
pod/argocd-notifications-controller-68459f6cbb-5sb9r   0/1     ContainerCreating   0          26s
pod/argocd-redis-794f68fb68-lw4cd                      0/1     Init:0/1            0          25s
pod/argocd-repo-server-864476c5cf-w6grd                0/1     Init:0/1            0          25s
pod/argocd-server-6496dc8859-x5glj                     0/1     ContainerCreating   0          25s

NAME                                              TYPE        CLUSTER-IP       EXTERNAL-IP   PORT(S)                      AGE
service/argocd-applicationset-controller          ClusterIP   10.98.216.163    <none>        7000/TCP,8080/TCP            26s
service/argocd-dex-server                         ClusterIP   10.102.98.54     <none>        5556/TCP,5557/TCP,5558/TCP   26s
service/argocd-metrics                            ClusterIP   10.96.252.241    <none>        8082/TCP                     26s
service/argocd-notifications-controller-metrics   ClusterIP   10.111.176.60    <none>        9001/TCP                     26s
service/argocd-redis                              ClusterIP   10.101.4.39      <none>        6379/TCP                     26s
service/argocd-repo-server                        ClusterIP   10.101.53.155    <none>        8081/TCP,8084/TCP            26s
service/argocd-server                             ClusterIP   10.110.80.4      <none>        80/TCP,443/TCP               26s
service/argocd-server-metrics                     ClusterIP   10.104.237.222   <none>        8083/TCP                     26s

NAME                                               READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/argocd-applicationset-controller   0/1     1            0           26s
deployment.apps/argocd-dex-server                  0/1     1            0           26s
deployment.apps/argocd-notifications-controller    0/1     1            0           26s
deployment.apps/argocd-redis                       0/1     1            0           25s
deployment.apps/argocd-repo-server                 0/1     1            0           25s
deployment.apps/argocd-server                      0/1     1            0           25s

NAME                                                         DESIRED   CURRENT   READY   AGE
replicaset.apps/argocd-applicationset-controller-9cbb56dff   1         1         0       26s
replicaset.apps/argocd-dex-server-74d5d76d7                  1         1         0       26s
replicaset.apps/argocd-notifications-controller-68459f6cbb   1         1         0       26s
replicaset.apps/argocd-redis-794f68fb68                      1         1         0       25s
replicaset.apps/argocd-repo-server-864476c5cf                1         1         0       25s
replicaset.apps/argocd-server-6496dc8859                     1         1         0       25s

NAME                                             READY   AGE
statefulset.apps/argocd-application-controller   0/1     25s
[root@masterbm ~]# kubectl get all --namespace=argocd
NAME                                                   READY   STATUS              RESTARTS   AGE
pod/argocd-application-controller-0                    0/1     ContainerCreating   0          27s
pod/argocd-applicationset-controller-9cbb56dff-9z2tj   0/1     ContainerCreating   0          28s
pod/argocd-dex-server-74d5d76d7-jhg4n                  0/1     Init:0/1            0          28s
pod/argocd-notifications-controller-68459f6cbb-5sb9r   0/1     ContainerCreating   0          28s
pod/argocd-redis-794f68fb68-lw4cd                      0/1     Init:0/1            0          27s
pod/argocd-repo-server-864476c5cf-w6grd                0/1     Init:0/1            0          27s
pod/argocd-server-6496dc8859-x5glj                     0/1     ContainerCreating   0          27s

NAME                                              TYPE        CLUSTER-IP       EXTERNAL-IP   PORT(S)                      AGE
service/argocd-applicationset-controller          ClusterIP   10.98.216.163    <none>        7000/TCP,8080/TCP            28s
service/argocd-dex-server                         ClusterIP   10.102.98.54     <none>        5556/TCP,5557/TCP,5558/TCP   28s
service/argocd-metrics                            ClusterIP   10.96.252.241    <none>        8082/TCP                     28s
service/argocd-notifications-controller-metrics   ClusterIP   10.111.176.60    <none>        9001/TCP                     28s
service/argocd-redis                              ClusterIP   10.101.4.39      <none>        6379/TCP                     28s
service/argocd-repo-server                        ClusterIP   10.101.53.155    <none>        8081/TCP,8084/TCP            28s
service/argocd-server                             ClusterIP   10.110.80.4      <none>        80/TCP,443/TCP               28s
service/argocd-server-metrics                     ClusterIP   10.104.237.222   <none>        8083/TCP                     28s

NAME                                               READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/argocd-applicationset-controller   0/1     1            0           28s
deployment.apps/argocd-dex-server                  0/1     1            0           28s
deployment.apps/argocd-notifications-controller    0/1     1            0           28s
deployment.apps/argocd-redis                       0/1     1            0           27s
deployment.apps/argocd-repo-server                 0/1     1            0           27s
deployment.apps/argocd-server                      0/1     1            0           27s

NAME                                                         DESIRED   CURRENT   READY   AGE
replicaset.apps/argocd-applicationset-controller-9cbb56dff   1         1         0       28s
replicaset.apps/argocd-dex-server-74d5d76d7                  1         1         0       28s
replicaset.apps/argocd-notifications-controller-68459f6cbb   1         1         0       28s
replicaset.apps/argocd-redis-794f68fb68                      1         1         0       27s
replicaset.apps/argocd-repo-server-864476c5cf                1         1         0       27s
replicaset.apps/argocd-server-6496dc8859                     1         1         0       27s

NAME                                             READY   AGE
statefulset.apps/argocd-application-controller   0/1     27s
[root@masterbm ~]# kubectl get all --namespace=argocd
NAME                                                   READY   STATUS              RESTARTS   AGE
pod/argocd-application-controller-0                    0/1     ContainerCreating   0          29s
pod/argocd-applicationset-controller-9cbb56dff-9z2tj   0/1     ContainerCreating   0          30s
pod/argocd-dex-server-74d5d76d7-jhg4n                  0/1     Init:0/1            0          30s
pod/argocd-notifications-controller-68459f6cbb-5sb9r   0/1     ContainerCreating   0          30s
pod/argocd-redis-794f68fb68-lw4cd                      0/1     Init:0/1            0          29s
pod/argocd-repo-server-864476c5cf-w6grd                0/1     Init:0/1            0          29s
pod/argocd-server-6496dc8859-x5glj                     0/1     ContainerCreating   0          29s

NAME                                              TYPE        CLUSTER-IP       EXTERNAL-IP   PORT(S)                      AGE
service/argocd-applicationset-controller          ClusterIP   10.98.216.163    <none>        7000/TCP,8080/TCP            30s
service/argocd-dex-server                         ClusterIP   10.102.98.54     <none>        5556/TCP,5557/TCP,5558/TCP   30s
service/argocd-metrics                            ClusterIP   10.96.252.241    <none>        8082/TCP                     30s
service/argocd-notifications-controller-metrics   ClusterIP   10.111.176.60    <none>        9001/TCP                     30s
service/argocd-redis                              ClusterIP   10.101.4.39      <none>        6379/TCP                     30s
service/argocd-repo-server                        ClusterIP   10.101.53.155    <none>        8081/TCP,8084/TCP            30s
service/argocd-server                             ClusterIP   10.110.80.4      <none>        80/TCP,443/TCP               30s
service/argocd-server-metrics                     ClusterIP   10.104.237.222   <none>        8083/TCP                     30s

NAME                                               READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/argocd-applicationset-controller   0/1     1            0           30s
deployment.apps/argocd-dex-server                  0/1     1            0           30s
deployment.apps/argocd-notifications-controller    0/1     1            0           30s
deployment.apps/argocd-redis                       0/1     1            0           29s
deployment.apps/argocd-repo-server                 0/1     1            0           29s
deployment.apps/argocd-server                      0/1     1            0           29s

NAME                                                         DESIRED   CURRENT   READY   AGE
replicaset.apps/argocd-applicationset-controller-9cbb56dff   1         1         0       30s
replicaset.apps/argocd-dex-server-74d5d76d7                  1         1         0       30s
replicaset.apps/argocd-notifications-controller-68459f6cbb   1         1         0       30s
replicaset.apps/argocd-redis-794f68fb68                      1         1         0       29s
replicaset.apps/argocd-repo-server-864476c5cf                1         1         0       29s
replicaset.apps/argocd-server-6496dc8859                     1         1         0       29s

NAME                                             READY   AGE
statefulset.apps/argocd-application-controller   0/1     29s
[root@masterbm ~]# kubectl get all --namespace=argocd
NAME                                                   READY   STATUS              RESTARTS   AGE
pod/argocd-application-controller-0                    0/1     ContainerCreating   0          31s
pod/argocd-applicationset-controller-9cbb56dff-9z2tj   0/1     ContainerCreating   0          32s
pod/argocd-dex-server-74d5d76d7-jhg4n                  0/1     Init:0/1            0          32s
pod/argocd-notifications-controller-68459f6cbb-5sb9r   0/1     ContainerCreating   0          32s
pod/argocd-redis-794f68fb68-lw4cd                      0/1     Init:0/1            0          31s
pod/argocd-repo-server-864476c5cf-w6grd                0/1     Init:0/1            0          31s
pod/argocd-server-6496dc8859-x5glj                     0/1     ContainerCreating   0          31s

NAME                                              TYPE        CLUSTER-IP       EXTERNAL-IP   PORT(S)                      AGE
service/argocd-applicationset-controller          ClusterIP   10.98.216.163    <none>        7000/TCP,8080/TCP            32s
service/argocd-dex-server                         ClusterIP   10.102.98.54     <none>        5556/TCP,5557/TCP,5558/TCP   32s
service/argocd-metrics                            ClusterIP   10.96.252.241    <none>        8082/TCP                     32s
service/argocd-notifications-controller-metrics   ClusterIP   10.111.176.60    <none>        9001/TCP                     32s
service/argocd-redis                              ClusterIP   10.101.4.39      <none>        6379/TCP                     32s
service/argocd-repo-server                        ClusterIP   10.101.53.155    <none>        8081/TCP,8084/TCP            32s
service/argocd-server                             ClusterIP   10.110.80.4      <none>        80/TCP,443/TCP               32s
service/argocd-server-metrics                     ClusterIP   10.104.237.222   <none>        8083/TCP                     32s

NAME                                               READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/argocd-applicationset-controller   0/1     1            0           32s
deployment.apps/argocd-dex-server                  0/1     1            0           32s
deployment.apps/argocd-notifications-controller    0/1     1            0           32s
deployment.apps/argocd-redis                       0/1     1            0           31s
deployment.apps/argocd-repo-server                 0/1     1            0           31s
deployment.apps/argocd-server                      0/1     1            0           31s

NAME                                                         DESIRED   CURRENT   READY   AGE
replicaset.apps/argocd-applicationset-controller-9cbb56dff   1         1         0       32s
replicaset.apps/argocd-dex-server-74d5d76d7                  1         1         0       32s
replicaset.apps/argocd-notifications-controller-68459f6cbb   1         1         0       32s
replicaset.apps/argocd-redis-794f68fb68                      1         1         0       31s
replicaset.apps/argocd-repo-server-864476c5cf                1         1         0       31s
replicaset.apps/argocd-server-6496dc8859                     1         1         0       31s

NAME                                             READY   AGE
statefulset.apps/argocd-application-controller   0/1     31s
[root@masterbm ~]# kubectl get all --namespace=argocd
NAME                                                   READY   STATUS    RESTARTS   AGE
pod/argocd-application-controller-0                    1/1     Running   0          83s
pod/argocd-applicationset-controller-9cbb56dff-9z2tj   1/1     Running   0          84s
pod/argocd-dex-server-74d5d76d7-jhg4n                  1/1     Running   0          84s
pod/argocd-notifications-controller-68459f6cbb-5sb9r   1/1     Running   0          84s
pod/argocd-redis-794f68fb68-lw4cd                      1/1     Running   0          83s
pod/argocd-repo-server-864476c5cf-w6grd                1/1     Running   0          83s
pod/argocd-server-6496dc8859-x5glj                     1/1     Running   0          83s

NAME                                              TYPE        CLUSTER-IP       EXTERNAL-IP   PORT(S)                      AGE
service/argocd-applicationset-controller          ClusterIP   10.98.216.163    <none>        7000/TCP,8080/TCP            84s
service/argocd-dex-server                         ClusterIP   10.102.98.54     <none>        5556/TCP,5557/TCP,5558/TCP   84s
service/argocd-metrics                            ClusterIP   10.96.252.241    <none>        8082/TCP                     84s
service/argocd-notifications-controller-metrics   ClusterIP   10.111.176.60    <none>        9001/TCP                     84s
service/argocd-redis                              ClusterIP   10.101.4.39      <none>        6379/TCP                     84s
service/argocd-repo-server                        ClusterIP   10.101.53.155    <none>        8081/TCP,8084/TCP            84s
service/argocd-server                             ClusterIP   10.110.80.4      <none>        80/TCP,443/TCP               84s
service/argocd-server-metrics                     ClusterIP   10.104.237.222   <none>        8083/TCP                     84s

NAME                                               READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/argocd-applicationset-controller   1/1     1            1           84s
deployment.apps/argocd-dex-server                  1/1     1            1           84s
deployment.apps/argocd-notifications-controller    1/1     1            1           84s
deployment.apps/argocd-redis                       1/1     1            1           83s
deployment.apps/argocd-repo-server                 1/1     1            1           83s
deployment.apps/argocd-server                      1/1     1            1           83s

NAME                                                         DESIRED   CURRENT   READY   AGE
replicaset.apps/argocd-applicationset-controller-9cbb56dff   1         1         1       84s
replicaset.apps/argocd-dex-server-74d5d76d7                  1         1         1       84s
replicaset.apps/argocd-notifications-controller-68459f6cbb   1         1         1       84s
replicaset.apps/argocd-redis-794f68fb68                      1         1         1       83s
replicaset.apps/argocd-repo-server-864476c5cf                1         1         1       83s
replicaset.apps/argocd-server-6496dc8859                     1         1         1       83s

NAME                                             READY   AGE
statefulset.apps/argocd-application-controller   1/1     83s
[root@masterbm ~]# kubectl get all --namespace=argocd
NAME                                                   READY   STATUS    RESTARTS   AGE
pod/argocd-application-controller-0                    1/1     Running   0          86s
pod/argocd-applicationset-controller-9cbb56dff-9z2tj   1/1     Running   0          87s
pod/argocd-dex-server-74d5d76d7-jhg4n                  1/1     Running   0          87s
pod/argocd-notifications-controller-68459f6cbb-5sb9r   1/1     Running   0          87s
pod/argocd-redis-794f68fb68-lw4cd                      1/1     Running   0          86s
pod/argocd-repo-server-864476c5cf-w6grd                1/1     Running   0          86s
pod/argocd-server-6496dc8859-x5glj                     1/1     Running   0          86s

NAME                                              TYPE        CLUSTER-IP       EXTERNAL-IP   PORT(S)                      AGE
service/argocd-applicationset-controller          ClusterIP   10.98.216.163    <none>        7000/TCP,8080/TCP            87s
service/argocd-dex-server                         ClusterIP   10.102.98.54     <none>        5556/TCP,5557/TCP,5558/TCP   87s
service/argocd-metrics                            ClusterIP   10.96.252.241    <none>        8082/TCP                     87s
service/argocd-notifications-controller-metrics   ClusterIP   10.111.176.60    <none>        9001/TCP                     87s
service/argocd-redis                              ClusterIP   10.101.4.39      <none>        6379/TCP                     87s
service/argocd-repo-server                        ClusterIP   10.101.53.155    <none>        8081/TCP,8084/TCP            87s
service/argocd-server                             ClusterIP   10.110.80.4      <none>        80/TCP,443/TCP               87s
service/argocd-server-metrics                     ClusterIP   10.104.237.222   <none>        8083/TCP                     87s

NAME                                               READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/argocd-applicationset-controller   1/1     1            1           87s
deployment.apps/argocd-dex-server                  1/1     1            1           87s
deployment.apps/argocd-notifications-controller    1/1     1            1           87s
deployment.apps/argocd-redis                       1/1     1            1           86s
deployment.apps/argocd-repo-server                 1/1     1            1           86s
deployment.apps/argocd-server                      1/1     1            1           86s

NAME                                                         DESIRED   CURRENT   READY   AGE
replicaset.apps/argocd-applicationset-controller-9cbb56dff   1         1         1       87s
replicaset.apps/argocd-dex-server-74d5d76d7                  1         1         1       87s
replicaset.apps/argocd-notifications-controller-68459f6cbb   1         1         1       87s
replicaset.apps/argocd-redis-794f68fb68                      1         1         1       86s
replicaset.apps/argocd-repo-server-864476c5cf                1         1         1       86s
replicaset.apps/argocd-server-6496dc8859                     1         1         1       86s

NAME                                             READY   AGE
statefulset.apps/argocd-application-controller   1/1     86s
[root@masterbm ~]# kubectl get all --namespace=argocd
NAME                                                   READY   STATUS    RESTARTS   AGE
pod/argocd-application-controller-0                    1/1     Running   0          87s
pod/argocd-applicationset-controller-9cbb56dff-9z2tj   1/1     Running   0          88s
pod/argocd-dex-server-74d5d76d7-jhg4n                  1/1     Running   0          88s
pod/argocd-notifications-controller-68459f6cbb-5sb9r   1/1     Running   0          88s
pod/argocd-redis-794f68fb68-lw4cd                      1/1     Running   0          87s
pod/argocd-repo-server-864476c5cf-w6grd                1/1     Running   0          87s
pod/argocd-server-6496dc8859-x5glj                     1/1     Running   0          87s

NAME                                              TYPE        CLUSTER-IP       EXTERNAL-IP   PORT(S)                      AGE
service/argocd-applicationset-controller          ClusterIP   10.98.216.163    <none>        7000/TCP,8080/TCP            88s
service/argocd-dex-server                         ClusterIP   10.102.98.54     <none>        5556/TCP,5557/TCP,5558/TCP   88s
service/argocd-metrics                            ClusterIP   10.96.252.241    <none>        8082/TCP                     88s
service/argocd-notifications-controller-metrics   ClusterIP   10.111.176.60    <none>        9001/TCP                     88s
service/argocd-redis                              ClusterIP   10.101.4.39      <none>        6379/TCP                     88s
service/argocd-repo-server                        ClusterIP   10.101.53.155    <none>        8081/TCP,8084/TCP            88s
service/argocd-server                             ClusterIP   10.110.80.4      <none>        80/TCP,443/TCP               88s
service/argocd-server-metrics                     ClusterIP   10.104.237.222   <none>        8083/TCP                     88s

NAME                                               READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/argocd-applicationset-controller   1/1     1            1           88s
deployment.apps/argocd-dex-server                  1/1     1            1           88s
deployment.apps/argocd-notifications-controller    1/1     1            1           88s
deployment.apps/argocd-redis                       1/1     1            1           87s
deployment.apps/argocd-repo-server                 1/1     1            1           87s
deployment.apps/argocd-server                      1/1     1            1           87s

NAME                                                         DESIRED   CURRENT   READY   AGE
replicaset.apps/argocd-applicationset-controller-9cbb56dff   1         1         1       88s
replicaset.apps/argocd-dex-server-74d5d76d7                  1         1         1       88s
replicaset.apps/argocd-notifications-controller-68459f6cbb   1         1         1       88s
replicaset.apps/argocd-redis-794f68fb68                      1         1         1       87s
replicaset.apps/argocd-repo-server-864476c5cf                1         1         1       87s
replicaset.apps/argocd-server-6496dc8859                     1         1         1       87s

NAME                                             READY   AGE
statefulset.apps/argocd-application-controller   1/1     87s
[root@masterbm ~]# kubectl get all --namespace=argocd
NAME                                                   READY   STATUS    RESTARTS   AGE
pod/argocd-application-controller-0                    1/1     Running   0          88s
pod/argocd-applicationset-controller-9cbb56dff-9z2tj   1/1     Running   0          89s
pod/argocd-dex-server-74d5d76d7-jhg4n                  1/1     Running   0          89s
pod/argocd-notifications-controller-68459f6cbb-5sb9r   1/1     Running   0          89s
pod/argocd-redis-794f68fb68-lw4cd                      1/1     Running   0          88s
pod/argocd-repo-server-864476c5cf-w6grd                1/1     Running   0          88s
pod/argocd-server-6496dc8859-x5glj                     1/1     Running   0          88s

NAME                                              TYPE        CLUSTER-IP       EXTERNAL-IP   PORT(S)                      AGE
service/argocd-applicationset-controller          ClusterIP   10.98.216.163    <none>        7000/TCP,8080/TCP            89s
service/argocd-dex-server                         ClusterIP   10.102.98.54     <none>        5556/TCP,5557/TCP,5558/TCP   89s
service/argocd-metrics                            ClusterIP   10.96.252.241    <none>        8082/TCP                     89s
service/argocd-notifications-controller-metrics   ClusterIP   10.111.176.60    <none>        9001/TCP                     89s
service/argocd-redis                              ClusterIP   10.101.4.39      <none>        6379/TCP                     89s
service/argocd-repo-server                        ClusterIP   10.101.53.155    <none>        8081/TCP,8084/TCP            89s
service/argocd-server                             ClusterIP   10.110.80.4      <none>        80/TCP,443/TCP               89s
service/argocd-server-metrics                     ClusterIP   10.104.237.222   <none>        8083/TCP                     89s

NAME                                               READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/argocd-applicationset-controller   1/1     1            1           89s
deployment.apps/argocd-dex-server                  1/1     1            1           89s
deployment.apps/argocd-notifications-controller    1/1     1            1           89s
deployment.apps/argocd-redis                       1/1     1            1           88s
deployment.apps/argocd-repo-server                 1/1     1            1           88s
deployment.apps/argocd-server                      1/1     1            1           88s

NAME                                                         DESIRED   CURRENT   READY   AGE
replicaset.apps/argocd-applicationset-controller-9cbb56dff   1         1         1       89s
replicaset.apps/argocd-dex-server-74d5d76d7                  1         1         1       89s
replicaset.apps/argocd-notifications-controller-68459f6cbb   1         1         1       89s
replicaset.apps/argocd-redis-794f68fb68                      1         1         1       88s
replicaset.apps/argocd-repo-server-864476c5cf                1         1         1       88s
replicaset.apps/argocd-server-6496dc8859                     1         1         1       88s

NAME                                             READY   AGE
statefulset.apps/argocd-application-controller   1/1     88s
[root@masterbm ~]# kubectl get all --namespace=argocd
NAME                                                   READY   STATUS    RESTARTS   AGE
pod/argocd-application-controller-0                    1/1     Running   0          90s
pod/argocd-applicationset-controller-9cbb56dff-9z2tj   1/1     Running   0          91s
pod/argocd-dex-server-74d5d76d7-jhg4n                  1/1     Running   0          91s
pod/argocd-notifications-controller-68459f6cbb-5sb9r   1/1     Running   0          91s
pod/argocd-redis-794f68fb68-lw4cd                      1/1     Running   0          90s
pod/argocd-repo-server-864476c5cf-w6grd                1/1     Running   0          90s
pod/argocd-server-6496dc8859-x5glj                     1/1     Running   0          90s

NAME                                              TYPE        CLUSTER-IP       EXTERNAL-IP   PORT(S)                      AGE
service/argocd-applicationset-controller          ClusterIP   10.98.216.163    <none>        7000/TCP,8080/TCP            91s
service/argocd-dex-server                         ClusterIP   10.102.98.54     <none>        5556/TCP,5557/TCP,5558/TCP   91s
service/argocd-metrics                            ClusterIP   10.96.252.241    <none>        8082/TCP                     91s
service/argocd-notifications-controller-metrics   ClusterIP   10.111.176.60    <none>        9001/TCP                     91s
service/argocd-redis                              ClusterIP   10.101.4.39      <none>        6379/TCP                     91s
service/argocd-repo-server                        ClusterIP   10.101.53.155    <none>        8081/TCP,8084/TCP            91s
service/argocd-server                             ClusterIP   10.110.80.4      <none>        80/TCP,443/TCP               91s
service/argocd-server-metrics                     ClusterIP   10.104.237.222   <none>        8083/TCP                     91s

NAME                                               READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/argocd-applicationset-controller   1/1     1            1           91s
deployment.apps/argocd-dex-server                  1/1     1            1           91s
deployment.apps/argocd-notifications-controller    1/1     1            1           91s
deployment.apps/argocd-redis                       1/1     1            1           90s
deployment.apps/argocd-repo-server                 1/1     1            1           90s
deployment.apps/argocd-server                      1/1     1            1           90s

NAME                                                         DESIRED   CURRENT   READY   AGE
replicaset.apps/argocd-applicationset-controller-9cbb56dff   1         1         1       91s
replicaset.apps/argocd-dex-server-74d5d76d7                  1         1         1       91s
replicaset.apps/argocd-notifications-controller-68459f6cbb   1         1         1       91s
replicaset.apps/argocd-redis-794f68fb68                      1         1         1       90s
replicaset.apps/argocd-repo-server-864476c5cf                1         1         1       90s
replicaset.apps/argocd-server-6496dc8859                     1         1         1       90s

NAME                                             READY   AGE
statefulset.apps/argocd-application-controller   1/1     90s
[root@masterbm ~]# kubectl get all --namespace=argocd
NAME                                                   READY   STATUS    RESTARTS   AGE
pod/argocd-application-controller-0                    1/1     Running   0          91s
pod/argocd-applicationset-controller-9cbb56dff-9z2tj   1/1     Running   0          92s
pod/argocd-dex-server-74d5d76d7-jhg4n                  1/1     Running   0          92s
pod/argocd-notifications-controller-68459f6cbb-5sb9r   1/1     Running   0          92s
pod/argocd-redis-794f68fb68-lw4cd                      1/1     Running   0          91s
pod/argocd-repo-server-864476c5cf-w6grd                1/1     Running   0          91s
pod/argocd-server-6496dc8859-x5glj                     1/1     Running   0          91s

NAME                                              TYPE        CLUSTER-IP       EXTERNAL-IP   PORT(S)                      AGE
service/argocd-applicationset-controller          ClusterIP   10.98.216.163    <none>        7000/TCP,8080/TCP            92s
service/argocd-dex-server                         ClusterIP   10.102.98.54     <none>        5556/TCP,5557/TCP,5558/TCP   92s
service/argocd-metrics                            ClusterIP   10.96.252.241    <none>        8082/TCP                     92s
service/argocd-notifications-controller-metrics   ClusterIP   10.111.176.60    <none>        9001/TCP                     92s
service/argocd-redis                              ClusterIP   10.101.4.39      <none>        6379/TCP                     92s
service/argocd-repo-server                        ClusterIP   10.101.53.155    <none>        8081/TCP,8084/TCP            92s
service/argocd-server                             ClusterIP   10.110.80.4      <none>        80/TCP,443/TCP               92s
service/argocd-server-metrics                     ClusterIP   10.104.237.222   <none>        8083/TCP                     92s

NAME                                               READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/argocd-applicationset-controller   1/1     1            1           92s
deployment.apps/argocd-dex-server                  1/1     1            1           92s
deployment.apps/argocd-notifications-controller    1/1     1            1           92s
deployment.apps/argocd-redis                       1/1     1            1           91s
deployment.apps/argocd-repo-server                 1/1     1            1           91s
deployment.apps/argocd-server                      1/1     1            1           91s

NAME                                                         DESIRED   CURRENT   READY   AGE
replicaset.apps/argocd-applicationset-controller-9cbb56dff   1         1         1       92s
replicaset.apps/argocd-dex-server-74d5d76d7                  1         1         1       92s
replicaset.apps/argocd-notifications-controller-68459f6cbb   1         1         1       92s
replicaset.apps/argocd-redis-794f68fb68                      1         1         1       91s
replicaset.apps/argocd-repo-server-864476c5cf                1         1         1       91s
replicaset.apps/argocd-server-6496dc8859                     1         1         1       91s

NAME                                             READY   AGE
statefulset.apps/argocd-application-controller   1/1     91s
[root@masterbm ~]# kubectl get all --namespace=argocd
NAME                                                   READY   STATUS    RESTARTS   AGE
pod/argocd-application-controller-0                    1/1     Running   0          93s
pod/argocd-applicationset-controller-9cbb56dff-9z2tj   1/1     Running   0          94s
pod/argocd-dex-server-74d5d76d7-jhg4n                  1/1     Running   0          94s
pod/argocd-notifications-controller-68459f6cbb-5sb9r   1/1     Running   0          94s
pod/argocd-redis-794f68fb68-lw4cd                      1/1     Running   0          93s
pod/argocd-repo-server-864476c5cf-w6grd                1/1     Running   0          93s
pod/argocd-server-6496dc8859-x5glj                     1/1     Running   0          93s

NAME                                              TYPE        CLUSTER-IP       EXTERNAL-IP   PORT(S)                      AGE
service/argocd-applicationset-controller          ClusterIP   10.98.216.163    <none>        7000/TCP,8080/TCP            94s
service/argocd-dex-server                         ClusterIP   10.102.98.54     <none>        5556/TCP,5557/TCP,5558/TCP   94s
service/argocd-metrics                            ClusterIP   10.96.252.241    <none>        8082/TCP                     94s
service/argocd-notifications-controller-metrics   ClusterIP   10.111.176.60    <none>        9001/TCP                     94s
service/argocd-redis                              ClusterIP   10.101.4.39      <none>        6379/TCP                     94s
service/argocd-repo-server                        ClusterIP   10.101.53.155    <none>        8081/TCP,8084/TCP            94s
service/argocd-server                             ClusterIP   10.110.80.4      <none>        80/TCP,443/TCP               94s
service/argocd-server-metrics                     ClusterIP   10.104.237.222   <none>        8083/TCP                     94s

NAME                                               READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/argocd-applicationset-controller   1/1     1            1           94s
deployment.apps/argocd-dex-server                  1/1     1            1           94s
deployment.apps/argocd-notifications-controller    1/1     1            1           94s
deployment.apps/argocd-redis                       1/1     1            1           93s
deployment.apps/argocd-repo-server                 1/1     1            1           93s
deployment.apps/argocd-server                      1/1     1            1           93s

NAME                                                         DESIRED   CURRENT   READY   AGE
replicaset.apps/argocd-applicationset-controller-9cbb56dff   1         1         1       94s
replicaset.apps/argocd-dex-server-74d5d76d7                  1         1         1       94s
replicaset.apps/argocd-notifications-controller-68459f6cbb   1         1         1       94s
replicaset.apps/argocd-redis-794f68fb68                      1         1         1       93s
replicaset.apps/argocd-repo-server-864476c5cf                1         1         1       93s
replicaset.apps/argocd-server-6496dc8859                     1         1         1       93s

NAME                                             READY   AGE
statefulset.apps/argocd-application-controller   1/1     93s
[root@masterbm ~]# kubectl get all --namespace=argocd
NAME                                                   READY   STATUS    RESTARTS   AGE
pod/argocd-application-controller-0                    1/1     Running   0          94s
pod/argocd-applicationset-controller-9cbb56dff-9z2tj   1/1     Running   0          95s
pod/argocd-dex-server-74d5d76d7-jhg4n                  1/1     Running   0          95s
pod/argocd-notifications-controller-68459f6cbb-5sb9r   1/1     Running   0          95s
pod/argocd-redis-794f68fb68-lw4cd                      1/1     Running   0          94s
pod/argocd-repo-server-864476c5cf-w6grd                1/1     Running   0          94s
pod/argocd-server-6496dc8859-x5glj                     1/1     Running   0          94s

NAME                                              TYPE        CLUSTER-IP       EXTERNAL-IP   PORT(S)                      AGE
service/argocd-applicationset-controller          ClusterIP   10.98.216.163    <none>        7000/TCP,8080/TCP            95s
service/argocd-dex-server                         ClusterIP   10.102.98.54     <none>        5556/TCP,5557/TCP,5558/TCP   95s
service/argocd-metrics                            ClusterIP   10.96.252.241    <none>        8082/TCP                     95s
service/argocd-notifications-controller-metrics   ClusterIP   10.111.176.60    <none>        9001/TCP                     95s
service/argocd-redis                              ClusterIP   10.101.4.39      <none>        6379/TCP                     95s
service/argocd-repo-server                        ClusterIP   10.101.53.155    <none>        8081/TCP,8084/TCP            95s
service/argocd-server                             ClusterIP   10.110.80.4      <none>        80/TCP,443/TCP               95s
service/argocd-server-metrics                     ClusterIP   10.104.237.222   <none>        8083/TCP                     95s

NAME                                               READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/argocd-applicationset-controller   1/1     1            1           95s
deployment.apps/argocd-dex-server                  1/1     1            1           95s
deployment.apps/argocd-notifications-controller    1/1     1            1           95s
deployment.apps/argocd-redis                       1/1     1            1           94s
deployment.apps/argocd-repo-server                 1/1     1            1           94s
deployment.apps/argocd-server                      1/1     1            1           94s

NAME                                                         DESIRED   CURRENT   READY   AGE
replicaset.apps/argocd-applicationset-controller-9cbb56dff   1         1         1       95s
replicaset.apps/argocd-dex-server-74d5d76d7                  1         1         1       95s
replicaset.apps/argocd-notifications-controller-68459f6cbb   1         1         1       95s
replicaset.apps/argocd-redis-794f68fb68                      1         1         1       94s
replicaset.apps/argocd-repo-server-864476c5cf                1         1         1       94s
replicaset.apps/argocd-server-6496dc8859                     1         1         1       94s

NAME                                             READY   AGE
statefulset.apps/argocd-application-controller   1/1     94s
[root@masterbm ~]# kubectl get all --namespace=argocd
NAME                                                   READY   STATUS    RESTARTS   AGE
pod/argocd-application-controller-0                    1/1     Running   0          96s
pod/argocd-applicationset-controller-9cbb56dff-9z2tj   1/1     Running   0          97s
pod/argocd-dex-server-74d5d76d7-jhg4n                  1/1     Running   0          97s
pod/argocd-notifications-controller-68459f6cbb-5sb9r   1/1     Running   0          97s
pod/argocd-redis-794f68fb68-lw4cd                      1/1     Running   0          96s
pod/argocd-repo-server-864476c5cf-w6grd                1/1     Running   0          96s
pod/argocd-server-6496dc8859-x5glj                     1/1     Running   0          96s

NAME                                              TYPE        CLUSTER-IP       EXTERNAL-IP   PORT(S)                      AGE
service/argocd-applicationset-controller          ClusterIP   10.98.216.163    <none>        7000/TCP,8080/TCP            97s
service/argocd-dex-server                         ClusterIP   10.102.98.54     <none>        5556/TCP,5557/TCP,5558/TCP   97s
service/argocd-metrics                            ClusterIP   10.96.252.241    <none>        8082/TCP                     97s
service/argocd-notifications-controller-metrics   ClusterIP   10.111.176.60    <none>        9001/TCP                     97s
service/argocd-redis                              ClusterIP   10.101.4.39      <none>        6379/TCP                     97s
service/argocd-repo-server                        ClusterIP   10.101.53.155    <none>        8081/TCP,8084/TCP            97s
service/argocd-server                             ClusterIP   10.110.80.4      <none>        80/TCP,443/TCP               97s
service/argocd-server-metrics                     ClusterIP   10.104.237.222   <none>        8083/TCP                     97s

NAME                                               READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/argocd-applicationset-controller   1/1     1            1           97s
deployment.apps/argocd-dex-server                  1/1     1            1           97s
deployment.apps/argocd-notifications-controller    1/1     1            1           97s
deployment.apps/argocd-redis                       1/1     1            1           96s
deployment.apps/argocd-repo-server                 1/1     1            1           96s
deployment.apps/argocd-server                      1/1     1            1           96s

NAME                                                         DESIRED   CURRENT   READY   AGE
replicaset.apps/argocd-applicationset-controller-9cbb56dff   1         1         1       97s
replicaset.apps/argocd-dex-server-74d5d76d7                  1         1         1       97s
replicaset.apps/argocd-notifications-controller-68459f6cbb   1         1         1       97s
replicaset.apps/argocd-redis-794f68fb68                      1         1         1       96s
replicaset.apps/argocd-repo-server-864476c5cf                1         1         1       96s
replicaset.apps/argocd-server-6496dc8859                     1         1         1       96s

NAME                                             READY   AGE
statefulset.apps/argocd-application-controller   1/1     96s
[root@masterbm ~]# curl -sSL -o argocd-linux-amd64 https://github.com/argoproj/argo-cd/releases/latest/download/argocd-linux-amd64
[root@masterbm ~]# sudo install -m 555 argocd-linux-amd64 /usr/local/bin/argocd
[root@masterbm ~]# rm argocd-linux-amd64
rm: remove regular file 'argocd-linux-amd64'? y
[root@masterbm ~]#

#HOW TO Login in argocd

[root@masterbm ~]# argocd admin  initial-password -n argocd
n7V0CabdjgIRu31T

 This password must be only used for first time login. We strongly recommend you update the password using `argocd account update-password`.
[root@masterbm ~]#




## Accessing Argo CD Services

```bash
kubectl get svc -n argocd

[root@masterbm ~]# kubectl get svc -n argocd
NAME                                      TYPE        CLUSTER-IP       EXTERNAL-IP   PORT(S)                      AGE
argocd-applicationset-controller          ClusterIP   10.98.216.163    <none>        7000/TCP,8080/TCP            56m
argocd-dex-server                         ClusterIP   10.102.98.54     <none>        5556/TCP,5557/TCP,5558/TCP   56m
argocd-metrics                            ClusterIP   10.96.252.241    <none>        8082/TCP                     56m
argocd-notifications-controller-metrics   ClusterIP   10.111.176.60    <none>        9001/TCP                     56m
argocd-redis                              ClusterIP   10.101.4.39      <none>        6379/TCP                     56m
argocd-repo-server                        ClusterIP   10.101.53.155    <none>        8081/TCP,8084/TCP            56m
argocd-server                             ClusterIP   10.110.80.4      <none>        80/TCP,443/TCP               56m
argocd-server-metrics                     ClusterIP   10.104.237.222   <none>        8083/TCP                     56m
[root@masterbm ~]#

kubectl port-forward svc/argocd-server 8080:443 -n argocd
kubectl port-forward --address 0.0.0.0 svc/argocd-server 8080:443 -n argocd
```
```bash

Port forward 

kubectl port-forward service/nameoftheservice local_port:target_port  
kubectl port-forward pod/nameofthepod local_port:target_port  


argocd-server                             ClusterIP   10.110.80.4      <none>        80/TCP,443/TCP   

kubectl port-forward service/argocd-server   :target_port        

[root@masterbm ~]# kubectl port-forward svc/argocd-server 8080:443 -n argocd
Forwarding from 127.0.0.1:8080 -> 8080
Forwarding from [::1]:8080 -> 8080
Handling connection for 8080
Handling connection for 8080
Handling connection for 8080
Handling connection for 8080
E0409 17:52:39.087410   93573 portforward.go:385] "Unhandled Error" err="error copying from remote stream to local connection: readfrom tcp6 [::1]:8080->[::1]:46358: write tcp6 [::1]:8080->[::1]:46358: write: broken pipe"
Handling connection for 8080



[root@masterbm ~]# argocd login localhost:8080
WARNING: server certificate had error: tls: failed to verify certificate: x509:                                                                        certificate signed by unknown authority. Proceed insecurely (y/n)? y
Username: admin
Password:
'admin:login' logged in successfully
Context 'localhost:8080' updated
[root@masterbm ~]#


logout
[root@masterbm ~]# argocd logout  localhost:8080
Logged out from 'localhost:8080'
[root@masterbm ~]#

cancel port forwarding 
[root@masterbm ~]# kubectl port-forward svc/argocd-server 8080:443 -n argocd
Forwarding from 127.0.0.1:8080 -> 8080
Forwarding from [::1]:8080 -> 8080
Handling connection for 8080
Handling connection for 8080
Handling connection for 8080
Handling connection for 8080
E0409 17:52:39.087410   93573 portforward.go:385] "Unhandled Error" err="error copying from remote stream to local connection: readfrom tcp6 [::1]:8080->[::1]:46358: write tcp6 [::1]:8080->[::1]:46358: write: broken pipe"
Handling connection for 8080
Handling connection for 8080
Handling connection for 8080
^C[root@masterbm ~]#
[root@masterbm ~]# argocd login localhost:8080
FATA[0000] dial tcp [::1]:8080: connect: connection refused
[root@masterbm ~]#

do curl try to open the url not openning 

^C[root@masterbm ~]# kubectport-forward svc/argocd-server 8080:44343 -n argocd
Forwarding from 127.0.0.1:8080 -> 8080
Forwarding from [::1]:8080 -> 8080
Handling connection for 8080

[root@masterbm ~]# curl  localhost:8080
<a href="https://localhost:8080/">Temporary Redirect</a>.


Another attempt to open argocd in web

^C[root@masterbm ~]kubectl port-forward --address 0.0.0.0 svc/argocd-server 8080:443 -n argocdcd
Forwarding from 0.0.0.0:8080 -> 8080
Handling connection for 8080
Handling connection for 8080
Handling connection for 8080
E0409 18:05:07.224530  101016 portforward.go:398] "Unhandled Error" err="error copying from local connection to remote stream: writeto tcp4 192.168.29.150:8080->192.168.29.23:40566: read tcp4 192.168.29.150:8080->192.168.29.23:40566: read: connection reset by peer"
Handling connection for 8080
Handling connection for 8080
Handling connection for 8080
Handling connection for 8080
Handling connection for 8080
Handling connection for 8080

root@masterbm ~]# curl  localhost:8080
<a href="https://localhost:8080/">Temporary Redirect</a>.

[root@masterbm ~]# ip -br a
lo               UNKNOWN        127.0.0.1/8 ::1/128
enp1s0           UP             192.168.29.150/24
cali1f3a91feb4d@if2 UP             fe80::ecee:eeff:feee:eeee/64
cali91dc23635c3@if2 UP             fe80::ecee:eeff:feee:eeee/64
cali0860c8522bc@if2 UP             fe80::ecee:eeff:feee:eeee/64
tunl0@NONE       UNKNOWN        172.16.149.128/32
[root@masterbm ~]#


[root@masterbm ~]# curl -v  -k  https://192.168.29.150:8080
*   Trying 192.168.29.150:8080...
* Connected to 192.168.29.150 (192.168.29.150) port 8080 (#0)
* ALPN, offering h2
* ALPN, offering http/1.1
*  CAfile: /etc/pki/tls/certs/ca-bundle.crt
* TLSv1.0 (OUT), TLS header, Certificate Status (22):
* TLSv1.3 (OUT), TLS handshake, Client hello (1):
* TLSv1.2 (IN), TLS header, Certificate Status (22):
* TLSv1.3 (IN), TLS handshake, Server hello (2):
* TLSv1.2 (IN), TLS header, Finished (20):
* TLSv1.2 (IN), TLS header, Unknown (23):
* TLSv1.3 (IN), TLS handshake, Encrypted Extensions (8):
* TLSv1.2 (IN), TLS header, Unknown (23):
* TLSv1.3 (IN), TLS handshake, Certificate (11):
* TLSv1.2 (IN), TLS header, Unknown (23):
* TLSv1.3 (IN), TLS handshake, CERT verify (15):
* TLSv1.2 (IN), TLS header, Unknown (23):
* TLSv1.3 (IN), TLS handshake, Finished (20):
* TLSv1.2 (OUT), TLS header, Finished (20):
* TLSv1.3 (OUT), TLS change cipher, Change cipher spec (1):
* TLSv1.2 (OUT), TLS header, Unknown (23):
* TLSv1.3 (OUT), TLS handshake, Finished (20):
* SSL connection using TLSv1.3 / TLS_AES_128_GCM_SHA256
* ALPN, server accepted to use http/1.1
* Server certificate:
*  subject: O=Argo CD
*  start date: Apr  9 10:43:51 2025 GMT
*  expire date: Apr  9 10:43:51 2026 GMT
*  issuer: O=Argo CD
*  SSL certificate verify result: self-signed certificate (18), continuing anyway.
* TLSv1.2 (OUT), TLS header, Unknown (23):
> GET / HTTP/1.1
> Host: 192.168.29.150:8080
> User-Agent: curl/7.76.1
> Accept: */*
>
* TLSv1.2 (IN), TLS header, Unknown (23):
* TLSv1.3 (IN), TLS handshake, Newsession Ticket (4):
* TLSv1.2 (IN), TLS header, Unknown (23):
* Mark bundle as not supporting multiuse
< HTTP/1.1 200 OK
< Accept-Ranges: bytes
< Content-Length: 788
< Content-Security-Policy: frame-ancestors 'self';
< Content-Type: text/html; charset=utf-8
< Vary: Accept-Encoding
< X-Frame-Options: sameorigin
< X-Xss-Protection: 1
< Date: Wed, 09 Apr 2025 12:36:52 GMT
<
* Connection #0 to host 192.168.29.150 left intact
<!doctype html><html lang="en"><head><meta charset="UTF-8"><title>Argo CD</title><base href="/"><meta name="viewport" content="width=device-width,initial-scale=1"><link rel="icon" type="image/png" href="assets/favicon/favicon-32x32.png" sizes="32x32"/><link rel="icon" type="image/png" href="assets/favicon/favicon-16x16.png" sizes="16x16"/><link href="assets/fonts.css" rel="stylesheet"><script defer="defer" src="main.67d3d35d60308e91d5f4.js"></script></head><body><noscript><p>Your browser does not support JavaScript. Please enable JavaScript to view the site. Alternatively, Argo CD can be used with the <a href="https://argoproj.github.io/argo-cd/cli_installation/">Argo CD CLI</a>.</p></noscript><div id="app"></div></body><script defer="defer" src="extensions.js"></script></html>[root@masterbm ~]#

```





 

