# WSUS

## 1Objetivo

WSUS se utiliza en el laboratorio para gestionar y probar la distribución centralizada de actualizaciones.

---

## Servidor

| Propiedad | Valor |
|---|---|
| Hostname | [HOST] |
| IP | [IP] |

---

## Grupos

| Grupo | Equipos |
|---|---|
| PILOT | [EQUIPOS] |
| PRODUCTION | [EQUIPOS] |

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

**GPO utilizada:**  
[NOMBRE]

**OU afectada:**  
[OU]

---

## Validación

-  Los clientes aparecen en WSUS.
    
-  Los clientes reciben la configuración.
    
-  Se comprueba el estado de actualizaciones.
    

---

## Resultado

[Descripción final.]
