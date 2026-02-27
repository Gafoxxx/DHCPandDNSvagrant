# DHCPandDNSvagrant
Playbook de Ansible idempotente y verificable que instala y configura DHCP (dhcpd) y DNS (BIND/named) en Rocky Linux 9.

JUAN FELIPE GARZÓN TREJOS
# Ansible Role: DNS (BIND) + DHCP en Rocky Linux 9

## Características

- Idempotente
- Validaciones: named-checkconf, named-checkzone, dhcpd -t
- Firewalld support
- Parametrización total vía group_vars
- Soporte interfaz DHCP estable vía /etc/sysconfig/dhcpd

## Uso

```bash
ansible-playbook site.yml
