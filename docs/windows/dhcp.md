# DHCP

## Objetivo

El servidor DHCP proporciona automáticamente:

- Dirección IP.
- Máscara.
- Gateway.
- DNS.
- Información del dominio.

---

## Scope

| Propiedad | Valor |
|---|---|
| Nombre | internal-scope |
| Inicio | 192.168.100.50 |
| Fin | 192.168.100.250 |

---

## Opciones DHCP

| Opción | Valor |
|---|---|
| Router | 192.168.1.1 |
| DNS | 192.168.20.10 |
| Dominio | opyee.net |

---

## Prueba de funcionamiento

Cliente utilizado:

- **CLI-WIN01**:

![Gateway ping](../../img/dhcp_win01_gatewayping.png)

![IP recibida - ping a WIN02](../../img/dhcp_ping_win01a02.png)

- **CLI-WIN02**:

![Gateway ping](../../img/dhcp_win02_gatewayping.png)

![IP recibida - ping a WIN01](../../img/dhcp_ping_win02a01.png)

- **DC01**:

![Concesiones de DHCP](../../img/DC01_DHCP.png)

---

## Validación

-  Cliente obtiene IP.
-  Gateway correcto.
-  DNS correcto.
-  Renovación DHCP correcta.

**CLI-WIN01**:

![ipconfig /all de CLI-WIN01](../../img/DHCP_IPCONFIGALL_WIN01.png)

**CLI-WIN02**:

![ipconfig /all de CLI-WIN02](../../img/DHCP_IPCONFIGALL_WIN02.png)

