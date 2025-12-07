[Volver al índice general](../README.md)

# UD1 – Análisis del entorno y detección de necesidades tecnológicas


![Debian](https://img.shields.io/badge/Debian-A81D33?style=for-the-badge&logo=debian&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/kubernetes-%23326ce5.svg?style=for-the-badge&logo=kubernetes&logoColor=white)
![Postgres](https://img.shields.io/badge/postgres-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white)
![Nginx](https://img.shields.io/badge/nginx-%23009639.svg?style=for-the-badge&logo=nginx&logoColor=white)
![Grafana](https://img.shields.io/badge/grafana-%23F46800.svg?style=for-the-badge&logo=grafana&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=Prometheus&logoColor=white)
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)


<p align="center">
  <img src="/UD1/img/analisis3.jpg" alt="![analisis3](/UD1/img/analisis3.jpg)" />
</p>  


# Índice de apartados
- [ ] [1. Análisis del sector tecnológico.](#1-análisis-del-sector-tecnológico)
- [ ] [2. Selección de la empresa o contexto de trabajo.](#2-selección-de-la-empresa-o-contexto-de-trabajo)
- [ ] [3. Identificación de necesidades tecnológicas.](#3-identificación-de-necesidades-tecnológicas)
- [ ] [4. Oportunidades y viabilidad del proyecto.](#4-oportunidades-y-viabilidad-del-proyecto)
- [ ] [5. Obligaciones legales y normativas.](#5-obligaciones-legales-y-normativas)
- [ ] [6. Guion inicial del proyecto.](#6-guion-inicial-del-proyecto)

      
# **1. Análisis del sector tecnológico**

El sector tecnológico en Sevilla se encuentra en plena transición hacia modelos de **Nube Híbrida** y entornos basados en **contenedores** (Docker/Kubernetes) ☁️. Los datos del **Sevilla TechPark (PCT Cartuja)** confirman esta consolidación: **575 empresas**, **más de 12.000 empleos** y un **11,1 % del PIB provincial** vinculado a tecnologías avanzadas 📊. Este crecimiento evidencia que la demanda de perfiles **ASIR** especializados en **administración de sistemas, ciberseguridad y automatización** seguirá aumentando, ya que las empresas buscan técnicos capaces de gestionar infraestructuras modernas y entornos cloud 🚀.

<p align="center">
  <img src="/UD1/img/grafica.png" alt="grafica" width="500" height="500">
</p>

Aun así, el mercado sevillano muestra una fuerte polarización 📊. Mientras las grandes consultoras concentran la mayor parte del talento, muchas PYMES mantienen infraestructuras obsoletas, sin **monitorización, copias de seguridad fiables o seguridad perimetral** 📉. Esta brecha digital abre una oportunidad clara para perfiles ASIR: un espacio poco cubierto donde aportar valor real implementando soluciones profesionales que **modernicen y protejan** a la pequeña empresa sevillana 🛠️💡.

 [⬆️ Volver al índice de apartados](#índice-de-apartados)

---

# **2. Selección de la empresa o contexto de trabajo**

<p align="center">
  <img src="/UD1/img/emergya.jpeg" alt="emergya" width="500" height="500">
</p>

* ### 🏢 Empresa Seleccionada: Emergya 

Para contextualizar el desarrollo de mi proyecto, he seleccionado como referente a **Emergya**, una empresa tecnológica ubicada en Nervión (Sevilla) que fue comprada por el grupo **Ayesa** 🏢 hace sólo un año. Lo que más me ha llamado la atención de esta compañía es que, dedicándose a un mundo digital tan exigente, su ADN sigue fundamentado en el **Software Libre** (con orígenes ligados a Guadalinex 🐧) y en el cuidado de su equipo bajo el lema *Digital & People* ❤️. Emergya prioriza el talento ofreciendo formación continua a sus empleados, para que sigan desarrollándose personal y profesionalmente, lo que consigue que esta empresa esté alejada del modelo de "rotación masiva" típico del sector y que disponga de un entorno de trabajo estable y motivador 🤝.

<p align="center">
  <img src="/UD1/img/emergya2.webp" alt="emergya2" width="400" height="400">
</p>

En el ámbito técnico son especialistas en **Cloud & Infraestructuras** y *Premier Partner* de Google Cloud, ayudando a grandes organizaciones a migrar sus servidores físicos a la nube ☁️. Su actividad abarca desde el desarrollo de plataformas web para el sector público hasta la implementación de soluciones de **Inteligencia Artificial** 🧠. Para mí son el espejo ideal, ya que su stack tecnológico valida las herramientas que quiero usar: trabajan con estándares como **Apache/Nginx**, gestionan bases de datos **PostgreSQL** y **MySQL** y dominan la **automatización** con **Python, Docker y Kubernetes** 📦.

[⬆️ Volver al índice de apartados](#índice-de-apartados)

---

# **3. Identificación de necesidades tecnológicas**

Analizando el contexto operativo de **Emergya** no es sencillo buscar puntos débiles en una empresa que lleva más de 20 años en el sector, pero a pesar de su excelencia técnica, y sabiendo que sólo hace un par de años de su compra por parte del grupo Ayesa, una unión de este calibre supone enfrentarse a un desafío crítico como es la **fragmentación de la infraestructura** 🧩.  Los administradores deben lidiar con la **gestión de entornos híbridos heterogéneos** donde conviven simultaneamente servidores físicos de proyectos antiguos con entornos modernos en **Google Cloud** lo que puede someter al equipo a una peligrosa **"Fatiga de Alertas"** 📉⚠️.

Para garantizar una observabilidad transversal detecto la necesidad de implementar una **Plataforma de Monitorización Centralizada** que funcione igual para los servidores físicos antiguos como para la nube ☁️. Mi propuesta técnica es desplegar un sistema basado en el **Stack TIG** (Telegraf, InfluxDB y Grafana), donde **Telegraf** será el encargado de extraer todas las métricas de todos los sistemas y centralizarlas en una única base de datos **InfluxDB** 🗄️. Así, los equipos de Emergya tendrán un **cuadro de mando único en Grafana** 🖥️ permitiéndoles controlar la salud de todos los activos del grupo independientemente de su origen y poder recibir **alertas automáticas ante saturaciones** 📊. 

[⬆️ Volver al índice de apartados](#índice-de-apartados)

---

# **4. Oportunidades y viabilidad del proyecto**

La viabilidad económica de esta propuesta es incuestionable, ya que se sustenta en un modelo de **coste cero en Licencias**. Al optar por el **Stack TIG** en sus versiones *Open Source (OSS)*, evitamos la adquisición de costosas suites de monitorización propietarias, lo que supone un importante ahorro económico de miles de euros anuales para la empresa 💰. Esto encaja perfectamente con la cultura de eficiencia de **Emergya**, ya que supone una inversión en talento interno, donde el único recurso necesario es el tiempo de configuración de los técnicos 📈.

Desde el punto de vista técnico, el proyecto es altamente viable y estratégico para el escenario de la fusión **Emergya-Ayesa**. La arquitectura es **ligera y agnóstica**. **Telegraf es capaz de ejecutarse tanto en los servidores antiguos como en los contenedores de **Google Cloud**, unificando la visión de ambos mundos sin necesidad de ampliar el hardware existente ⚡. Implementar esta solución resuelve el problema de la fragmentación de forma gratuita y dota a la compañía de una plataforma de **observabilidad propia y escalable**, garantizando la sostenibilidad tecnológica a largo plazo 🛡️.

<p align="center">
  <img src="/UD1/img/stacktig.png" alt="stacktig">
</p>

[⬆️ Volver al índice de apartados](#índice-de-apartados)

---

# **5. Obligaciones legales y normativas**

El despliegue en **Emergya** exige un estricto cumplimiento del **Esquema Nacional de Seguridad (ENS)** al operar infraestructuras críticas para la Administración Pública, cumpliendo rigurosamente sus principios de confidencialidad, integridad, disponibilidad y trazabilidad 🛡️. La centralización de logs y métricas conlleva el tratamiento de datos personales (direcciones IP, identificadores de usuario), lo que activa el cumplimiento del **RGPD** y la **LOPD-GDD** ⚖️. Esto exige aplicar medidas técnicas concretas, como el cifrado de datos en reposo en la base de datos, controles de acceso basados en roles (RBAC) y la firma de acuerdos de confidencialidad por parte del personal técnico con acceso a los paneles.

En materia de Propiedad Intelectual, el uso del **Stack TIG** requiere respetar un marco de licencias mixtas 🐧📄:

* Telegraf: Se distribuye bajo licencia permisiva MIT.  
* InfluxDB OSS: Utiliza una combinación de licencia MIT para el motor y EULA para ciertos componentes.  
* Grafana: Se rige por la licencia AGPLv3. Esta licencia obligaría a publicar el código si redistribuyéramos una versión modificada; sin embargo, al utilizar la herramienta sin alteraciones de código fuente, operamos dentro de la legalidad sin generar obligaciones adicionales.

Finalmente, cumplimos con el **RD 488/1997 de Prevención de Riesgos Laborales (PRL)** aplicando medidas de ergonomía digital, como el uso de "Modos Oscuros" y alertas inteligentes para reducir la fatiga visual y operativa del equipo técnico 🖥️👀.


[⬆️ Volver al índice de apartados](#índice-de-apartados)

---
 
# **6. Guion inicial del proyecto**

A continuación detallo la hoja de ruta técnica para la ejecución del proyecto **Observabilidad Híbrida con Stack TIG en Emergya**, estructurada en cuatro fases secuenciales que garantizan el control del ciclo de vida del dato y la seguridad de la infraestructura.

**FASE 1: ARQUITECTURA Y DISEÑO 🏗️**

El objetivo de esta fase es establecer los cimientos lógicos del proyecto antes de desplegar cualquier activo.

  * **Auditoría de Activos:** Realización de un inventario exhaustivo de los servidores Legacy (On-Premise) y los recursos Cloud (Google Cloud Platform) de Emergya para identificar los puntos críticos de monitorización.

  * **Diseño de Red Segura:** Definición de la segmentación de red para aislar el tráfico de monitorización y diseño de las reglas de Firewall para proteger el entorno.

  * **Selección de Software:** Validación de las versiones Open Source (OSS) del Stack TIG (Telegraf, InfluxDB, Grafana) para asegurar la compatibilidad con el sistema base.

**FASE 2: APROVISIONAMIENTO E INFRAESTRUCTURA ☁️**

En esta etapa despliego la base tecnológica sobre la que correrán los servicios.

  * **Servidor (VPS):** Despliegue de un Servidor Privado Virtual con sistema operativo Debian 12 (Bookworm) priorizando la estabilidad y el soporte a largo plazo.

  * **Hardening de Seguridad:** Aplicación de medidas de endurecimiento del sistema incluyendo autenticación por SSH y configuración contra intrusiones.

  * **Capa de Contenedores:** Instalación y configuración de **Docker Engine** y **Docker Compose** creando redes internas (Bridge Networks) para aislar los servicios.

  * **Persistencia de Datos:** Configuración de volúmenes cifrados para la base de datos **InfluxDB** (series temporales) y **PostgreSQL** (gestión de usuarios) garantizando la integridad de la información ante reinicios.

**FASE 3: IMPLEMENTACIÓN DEL STACK (EL CEREBRO) ⚙️**

Fase central donde se configura la lógica de la observabilidad.

  * **Recolección (Telegraf):** Despliegue del agente recolector y configuración de inputs para monitorizar métricas de sistema (CPU, RAM, Disco) y servicios web (Nginx). 

  * **Almacenamiento (InfluxDB):** Configuración de las Políticas de Retención para gestionar el ciclo de vida de los datos y gestión de Tokens de seguridad para el acceso a la API.

  * **Visualización (Grafana):** Conexión segura con las fuentes de datos, diseño de Dashboards con ergonomía visual ("Modo Oscuro") y configuración de un sistema de Alertas Inteligentes vía Telegram/Email para evitar la fatiga de alertas.

**FASE 4: VALIDACIÓN Y CIERRE 📝**

Etapa final para asegurar la calidad y el cumplimiento normativo.

  * **Auditoría de Cumplimiento:** Verificación técnica del cifrado de datos personales para cumplir con el RGPD y revisión de las licencias de software.

  * **Pruebas de Estrés:** Ejecución de simulacros de caída de servicios para validar la respuesta automática del sistema de alertas.

  * **Documentación Final:** Elaboración del "Manual de Despliegue" y la "Guía de Usuario" para facilitar la transferencia de conocimiento al equipo técnico de Emergya.

📂 PROYECTO: OBSERVABILIDAD HÍBRIDA (STACK TIG) - EMERGYA  
│
├─ 🏗️ FASE 1: ARQUITECTURA Y DISEÑO  
│   ├──── 🔍 Auditoría de Activos  
│   │   ├────── Inventariado de servidores Legacy (On-Premise)  
│   │   └────── Análisis de recursos Cloud (Google Cloud)  
│   │  
│   ├──── 📐 Diseño de Red  
│   │   ├────── Segmentación de tráfico de monitorización  
│   │   └────── Definición de reglas de Firewall   
│   │  
│   └──── 📦 Selección de Software  
│       └────── Validación de versiones OSS (Telegraf, InfluxDB, Grafana)  
│  
├─ ☁️ FASE 2: APROVISIONAMIENTO E INFRAESTRUCTURA  
│   ├──── 🐧 Servidor Core  
│   │   ├────── Despliegue de VPS con Debian 12 (Bookworm)  
│   │   └────── Hardening de seguridad (SSH)  
│   │  
│   ├──── 🐳 Capa de Contenedores  
│   │   ├────── Instalación de Docker Engine & Docker Compose  
│   │   └────── Creación de redes internas (Bridge Network)  
│   │  
│   └──── 💾 Persistencia de Datos  
│       ├────── Volúmenes cifrados para InfluxDB (Series Temporales)  
│       └────── PostgreSQL para gestión de usuarios  
│  
├─ ⚙️ FASE 3: IMPLEMENTACIÓN DEL STACK TIG  
│   ├──── 📡 Recolección (Telegraf)  
│   │   └────── Configuración de inputs (CPU, RAM, Disco, Nginx)  
│   │  
│   ├──── 🗄️ Almacenamiento (InfluxDB)  
│   │   ├────── Configuración de retención de datos  
│   │   └────── Token management para seguridad  
│   │  
│   └──── 🖥️ Visualización (Grafana)  
│       ├────── Conexión segura con Data Sources  
│       ├────── Diseño de Dashboards "Modo Oscuro" (Ergonomía)  
│       └────── Sistema de Alertas Inteligentes (Telegram/Email)  
│  
└─ 📝 FASE 4: VALIDACIÓN Y CIERRE  
    ├──── 🛡️ Auditoría de Cumplimiento  
    │   ├────── Verificación de cifrado (RGPD)  
    │   └────── Revisión de licencias (Compliance)  
    │  
    ├──── 💣 Pruebas de Estrés  
    │   └────── Simulación de caída de servicios y respuesta de alertas  
    │  
    └──── 📄 Documentación Final  
        ├────── Manual de Despliegue  
        └────── Guía de Usuario para técnicos de Emergya  

[⬆️ Volver al índice de apartados](#índice-de-apartados) 

---

## Enlaces a recursos de la unidad

- [Documentos de la unidad](./documentos/)

- [Diagramas e imágenes](./img/)

## Bibliografía / Webgrafía


- Servicio Público de Empleo Estatal (SEPE). (2024). Informes anuales del mercado de trabajo provincial: Sevilla. Ministerio de Trabajo y Economía Social.  
    🔗 [Acceder al informe oficial del SEPE](https://www.sepe.es/HomeSepe/que-es-observatorio/informes-anuales-mercado-trabajo-provincial-municipal/informes-provincia/ver-resultados.html?documentType=informes&tipo=9&ambito=Provincial&provincia=41)
  
- Parque Científico y Tecnológico Cartuja (Sevilla TechPark). (2025). Informe de Evolución y Desarrollo Tecnológico y Económico. Junta de Andalucía.  
    🔗 [Acceder a la sección de Informes y Memorias](https://sevillatechpark.es/sevilla-techpark/#en-cifras)  
    🔗 [Sevilla TechPark](https://www.youtube.com/watch?v=HjEJF6tb8hI)  
    *(Nota: Fuente de los datos de facturación y empleo del parque).*

- Cámara de Comercio de Sevilla. (2024/2025). Informes de Coyuntura Socioeconómica.  
    🔗 [Acceder al informe del 3er trimestre](https://fundacioncamaradesevilla.com/eventos/527036/)

- Web Corporativa de Emergya  
    🔗 [Área de Trabajo](https://www.emergya.com/es/efecto-emergya))
        
- Google Cloud Partner  
    🔗 [Perfil oficial de Partner](https://cloud.google.com/find-a-partner/partner/emergya-digital)

- Cultura "People" Emergya  
    🔗 [Emergya Careers](https://www.emergya.com/es/trabaja-con-nosotros)  

- Funtes Oficiales Normativas:  
    🔗 [RD 488/1997 (Pantallas)](https://www.boe.es/buscar/act.php?id=BOE-A-1997-8669)    
    🔗 [Licencia AGPLv3 de Grafana](https://grafana.com/blog/2021/04/20/grafana-loki-tempo-relicensing-to-agplv3/)  
    🔗 [ENS (Esquema Nacional de Seguridad)](https://www.ccn-cert.cni.es/es/series-ccn-stic/documentos-publicos/ens/2449-femp-ens-tomo-1-guia-estrategica-en-seguridad-para-entidades-locales/file.html)
