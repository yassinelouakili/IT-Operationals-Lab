# IT Operations Lab

Laboratorio de infraestructura IT montado en VirtualBox para practicar competencias en: Active Directory, redes, monitorización, automatización y gestión de incidencias ITIL.

---

## Objetivo
El objetivo de este proyecto es preparar un laboratorio para aprender/mejorar

---

## Arquitectura 

![DIAGRAMA DE LA INFRAESTRUCTURA](img/ITOperationalLab_Diagram.png)

Documentación detallada en:
- [Arquitectura](docs/arquitectura.md)
- [Direccionamiento IP](docs/direccionamiento.md)
- [Inventario](docs/inventario.md)

---

## Sistemas

| Hostname | Sistema Operativo | Función |
| -------- | ----------------- | ------- |
| FW-pfSense | pfSense 2.9.0 | Firewall del laboratorio y Segmentación de red |
| DC01 | Windows Server 2025 | Servidor principal del laboratorio |
| MON-ZBX | Ubuntu Server 26.04 | Monitorizar con Zabbix |
| SUP-UBUDESK | Ubuntu Desktop 26.04 | Simulación de soporte técnico |
| CLI-WIN01 | Windows 11 | Simulación de cliente |
| CLI-WIN02 | Windows 11 | Simulación de cliente |

---

## Estructura del proyecto
```text
it-operations-lab/  
├── README.md   
└── docs    
    ├── arquitectura.md 
    ├── direccionamiento.md 
    ├── inventario.md
    └── network
        └── pfsense.md
```

---

## Documentación 
La documentación completa está disponible en la carpeta [docs](docs)

--- 
### Autor
Yassine Elouakili El Mahdati
