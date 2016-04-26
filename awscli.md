awscli
======

```bash
$ --query 'Reservations[].Instances[].[Tags,InstanceId]'
$ --query 'RouteTables[].[Tags,RouteTableId]'
$ --query 'InternetGateways[].[Tags,InternetGatewayId]'
$ --query 'Subnets[].[Tags,SubnetId]'
$ curl http://169.254.169.254/latest/meta-data/
$ curl http://169.254.169.254/latest/meta-data/local-ipv4
$ curl http://169.254.169.254/latest/meta-data/public-ipv4
$ curl http://169.254.169.254/latest/meta-data/instance-id
```
