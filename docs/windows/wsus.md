# WSUS

## Objetivo

WSUS se utiliza en el laboratorio para gestionar y probar la distribución centralizada de actualizaciones.

---

## Servidor

| Propiedad | Valor |
|---|---|
| Hostname | [DC01] |
| IP | [192.168.20.10] |

---

## Grupos

| Grupo | Equipos |
|---|---|
| PILOT | [CLI-WIN01] - equipos de prueba |
| PRODUCTION | [CLI-WIN02] - equipos de cliente real |

El grupo `PILOT` recibe primero las actualizaciones para comprobar que no aparecen problemas. Una vez validado, las actualizaciones se aprueban para el grupo `PRODUCTION`

---

## Flujo de actualizaciones

```text
Microsoft Update
        ↓
WSUS
        ↓
PILOT
        ↓
Validación
        ↓
PRODUCTION
````

---

## Configuración mediante GPO

**GPO utilizada:** [GPO-003-Windows-Update]

**OU afectada:** [Equipos]

---

## Validación

-  Los clientes aparecen en WSUS.
    
-  Los clientes reciben la configuración.
    
-  Se comprueba el estado de actualizaciones.
    
