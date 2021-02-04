# Ansible Role Kafka Admin

Ansible role to configure various admin tools for Apache Kafka such as:

- Zoonavigator
- Kafka Manager

These applications will run within docker containers, but the role
also installs docker and all dependencies.

## Requirements

The firewall on the Kafka admin server needs to have port 80 open to access the
nginx webserver.

The zookeeper and kafka servers also need to allow access to the kafka admin
server as follows:

| Servers   | Port to allow Kafka Admin Access |
|-----------|----------------------------------|
| Kafka     | 9092                             |
| Zookeeper | 2181                             |

## Role Variables

kafka_admin_zookeeper_hosts: 127.0.0.1:2181

This is a comma separated list of your zookeeper hosts.

## Dependencies

NONE

## Example Playbook

```yml
```

## License

GPLv2

## Author Information

Ashley Kleynhans
