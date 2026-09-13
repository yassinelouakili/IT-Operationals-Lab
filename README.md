    # IT Operationals Lab

    Laboratorio de infraestructura IT virtualizada orientado a reproducir un entorno corporativo. Administración de Active Directory, configuración de redes, monitorización con Zabbix, automatización de procesos y gestión de incidencias siguiendo buenas prácticas ITIL

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
    ├── network
    |   └── pfsense.md
    ├── windows/
    |   ├── active-directory.md
    |   ├── dns.md
    |   ├── dhcp.md
    |   ├── gpo.md
    |   └── wsus.md
    |
    └── monitoring/
        └── zabbix.md
    ```

    ---

    ## Documentación 
    La documentación completa está disponible en la carpeta [docs](docs)

    --- 
    ### Autor
    Yassine Elouakili El Mahdati
