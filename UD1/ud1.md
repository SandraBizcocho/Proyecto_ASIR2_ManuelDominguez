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
- [ ] [4. Oportunidades y viabilidad del proyecto.]
- [ ] [5. Obligaciones legales y normativas.]
- [ ] [6. Guion inicial del proyecto.]

      
# **1. Análisis del sector tecnológico**

El sector tecnológico en Sevilla se encuentra en plena transición hacia modelos de **Nube Híbrida** y entornos basados en **contenedores** (Docker/Kubernetes) ☁️. Los datos del **Sevilla TechPark (PCT Cartuja)** confirman esta consolidación: **575 empresas**, **más de 12.000 empleos** y un **11,1 % del PIB provincial** vinculado a tecnologías avanzadas 📊. Este crecimiento evidencia que la demanda de perfiles **ASIR** especializados en **administración de sistemas, ciberseguridad y automatización** seguirá aumentando, ya que las empresas buscan técnicos capaces de gestionar infraestructuras modernas y entornos cloud 🚀.

<p align="center">
  <img src="/UD1/img/grafica.png" alt="grafica" width="500" height="500">
</p>

Aun así, el mercado sevillano muestra una fuerte polarización 📊. Mientras las grandes consultoras concentran la mayor parte del talento, muchas PYMES mantienen infraestructuras obsoletas, sin **monitorización, copias de seguridad fiables o seguridad perimetral** 📉. Esta brecha digital abre una oportunidad clara para perfiles ASIR: un espacio poco cubierto donde aportar valor real implementando soluciones profesionales que **modernicen y protejan** a la pequeña empresa sevillana 🛠️💡.

 [⬆️ Volver al índice de apartados](#índice-de-apartados)

---

# **2. Selección de la empresa o contexto de trabajo**

* ### 🏢 Empresa Seleccionada: Emergya <img src="/UD1/img/emergya.jpeg" alt="emergya" width="200" height="200">

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



# **6. Guion inicial del proyecto**


 [⬆️ Volver al índice de apartados](#índice-de-apartados) 


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
