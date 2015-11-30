awscli
======

```bash
$ --query 'Reservations[].Instances[].[Tags,InstanceId]'
$ --query 'RouteTables[].[Tags,RouteTableId]'
$ --query 'InternetGateways[].[Tags,InternetGatewayId]'
$ --query 'Subnets[].[Tags,SubnetId]'
```
