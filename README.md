# Percona XtraDB Cluster + ProxySQL on Kubernetes / Openshift

The goal of this project is to provide a complete install path for Percona XtraDB Cluster + ProxySQL on Kubernetes / Openshift.
* pxc-k8s/ includes Percona XtraDB Cluster docker for Kubernetes / Openshift (fork from https://github.com/Percona-Lab/percona-docker/tree/master/pxc-k8s). It uses the new version of discovery service (does not rely on ETCD anymore)
* proxysql-k8s/ is the new version of proxysql + discovery service for Percona XtraDB Cluster nodes
* pxc_proxy.yaml is the YAML for kubernetes / openshift. For openshift run: oc new-project pxc-proxy; oc create -f pxc_proxy.yaml

