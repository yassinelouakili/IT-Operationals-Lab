# DNS

## Objetivo

El servicio DNS proporciona:

- Resolución de nombres internos.
- Resolución de nombres externos mediante [forwarders/configuración].

---

## Servidor

| Propiedad | Valor |
|---|---|
| Hostname | [DC01] |
| IP | [192.168.20.10] |

---

## Zona principal

```text
[opyee.net]
```

---

## Configuración

### Forwarders

[192.168.1.1, 8.8.8.8]

### Registros relevantes

| Nombre | Tipo | Dirección |
|---|---|---|
| CLI-WIN01 | Cliente | DHCP |
| CLI-WIN02 | Cliente | DHCP |

---

## Pruebas

![Ping interno y externo desde WIN02](../../img/DNS_InternalExternalPing.png)