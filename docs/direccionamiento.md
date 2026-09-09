# Plan de direccionamiento IP

## 1. Red LAN

| Propiedad | Valor |
|---|---|
| Red | 192.168.0.0 |
| Máscara | 255.255.0.0 |
| Gateway | 192.168.1.1 |
| Rango DHCP | 192.168.100.50 - 250 |

---

## 2. Direcciones estáticas

| Hostname | IP | Función |
|---|---|---|
| FW-pfSense | 192.168.1.1 | Firewall y gateway |
| DC01 | 192.168.20.10 | AD, DNS, DHCP, GPO y WSUS |
| MON-ZBX | 192.168.20.20 | Monitorización con Zabbix |
| SUP-UBUDESK | 192.168.40.10 | Soporte y ticketing |

--- 

## 3. DHCP

### Scope

| Configuración | Valor |
|---|---|
| Nombre | LAN |
| Rango | 192.168.100.50 - 192.168.100.250 |
| Gateway | 192.168.1.1 |
| DNS | 192.168.20.10 |
| Dominio | [opyee.net] |

El DHCP asigna automáticamente a los clientes su dirección IP, gateway y servidor DNS.


--- 

## 5. DNS

El servidor DNS principal es `DC01`.
Servidor DNS principal: `192.168.20.10`.
Dominio interno: `opyee.net`.

El DNS permite que los equipos del laboratorio puedan localizar los servidores y servicios utilizando nombres en lugar de tener que utilizar directamente sus direcciones IP.

## 6. Notas
- Las direcciones de los servidores se mantienen fuera del rango DHCP para evitar conflictos.
- Los equipos cliente utilizan DHCP.
- `DC01` se utiliza como DNS principal para los equipos del dominio.
- `FW-pfSense` actúa como gateway de la red.
- El rango `192.168.100.0/24` se reserva para las direcciones asignadas dinámicamente.
- La red `192.168.0.0/16` deja espacio para añadir nuevas redes o segmentos en futuras versiones.
