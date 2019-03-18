# ingress

This role configures an NGINX ingress in a cluster.

## Variables

You can set the following variables.

|Name|Default value|Description|
|----|-------------|-----------|
|`ingress_nginx_version`|0.23.0|The NGINX ingress version to deploy.|
|`ingress_nginx_tcp_ports`|[]|A list of tcp ports to map, entries must be of the form `{ port: <int>, service: <namespace>/<service> }`.
|`ingress_nginx_udp_ports`|[]|A list of udp ports to map, entries must be of the form `{ port: <int>, service: <namespace>/<service> }`.
|`ingress_nginx_resource_state`|present|Whether to deploy
|`ingress_nginx_resource_kubeconfig`|~/.kube/config|Path to the kubeconfig to use.|
|`ingress_nginx_namespace`|ingress-nginx|The name of the created namespace.|
|`ingress_nginx_serviceaccount`|ingress-nginx|The name of the created serviceaccount.|
|`ingress_nginx_role`|ingress-nginx|The name of the created role.|
|`ingress_nginx_rolebinding`|ingress-nginx|The name of the created role binding.|
|`ingress_nginx_clusterrole`|ingress-nginx|The name of the created cluster role.|
|`ingress_nginx_clusterrolebinding`|ingress-nginx|The name of the created cluster role binding.|
|`ingress_nginx_daemonset_name`|ingress-nginx|The name of the created DaemonSet.|
