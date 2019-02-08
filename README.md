# ingress

This role configures an NGINX ingress in a cluster.

## Variables

You can set the following variables.

|Name|Default value|Description|
|----|-------------|-----------|
|`ingress_nginx_version`|0.22.0|The ingress-nginx version to deploy.|
|`ingress_nginx_tcp_ports`|[]|A list of tcp ports to map, entries must be of the form `{ port: <int>, service: <namespace>/<service> }`.
|`ingress_nginx_udp_ports`|[]|A list of udp ports to map, entries must be of the form `{ port: <int>, service: <namespace>/<service> }`.
