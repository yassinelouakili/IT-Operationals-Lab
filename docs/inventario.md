# Inventario de infraestructura

## Sistemas

| Hostname | Sistema operativo | IP | Función | Estado |
|---|---|---|---|---|
| pfSense | pfSense 2.9.0 | LAN: 192.168.1.1/16 | Firewall, Segmentación de red | [En creación] |
| DC01 | Windows Server 2025 | 192.168.20.10/16 | Active Directory, DHCP, DNS, WSUS | [En creación] |
| MON-ZBX | Ubuntu Server 26.04 | 192.168.20.20/16 | Monitorización de sistemas | [En creación] |
| SUP-UBUDESK | Ubuntu Desktop 26.04 | 192.168.40.10/16 | Simulación de soporte técnico | [En creación] |
| CLI-WIN01 | Windows 11 | 192.168.100.50-250/16 | Simulación de cliente | [En creación] |
| CLI-WIN02 | Windows 11 | 192.168.100.50-250/16 | Simulación de cliente | [En creación] |

---

## Servicios


| Servicio | Host | Descripción |
|---|---|---|
| Firewall | pfSense | Control del tráfico de red |
| Active Directory | DC01 | Gestión de usuarios, grupos y equipos |
| DNS | DC01 | Resolución de nombres del laboratorio |
| DHCP | DC01 | Asignación automática de direcciones IP |
| WSUS | DC01 | Gestión de actualizaciones de Windows |
| Zabbix | MON-ZBX | Monitorización de sistemas |
| Ticketing | SUP-UBUDESK | Gestión de incidencias de soporte |


---

## Recursos asignados

| Host | RAM | CPU | Disco |
|---|---|---|---|
| pfSense | 2GB | 2 | 16GB |
| DC01 | 6GB | 2 | 100GB |
| MON-ZBX | 4GB | 2 | 25GB |
| SUP-UBUDESK | 2GB | 2 | 25GB |
| CLI-WIN01 | 4GB | 2 | 80GB |
| CLI-WIN02 | 4GB | 2 | 80GB |


---

## Software relevante

| Software | Sistema | Uso |
|---|---|---|
| pfSense | pfSense | Firewall y gestión de red |
| Active Directory | DC01 | Gestión del dominio |
| DNS | DC01 | Resolución de nombres |
| DHCP | DC01 | Asignación de IP |
| WSUS | DC01 | Gestión de actualizaciones |
| Zabbix | MON-ZBX | Monitorización |
| Ticketing | SUP-UBUDESK | Gestión de incidencias |


---

## Última revisión
[01/09/2026]











