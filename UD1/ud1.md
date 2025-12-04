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
  <img src="/UD1/img/tabla.png" alt="![tabla](/UD1/img/tabla.png)" />
</p>

Aun así, el mercado sevillano muestra una fuerte polarización 📊. Mientras las grandes consultoras concentran la mayor parte del talento, muchas PYMES mantienen infraestructuras obsoletas, sin **monitorización, copias de seguridad fiables o seguridad perimetral** 📉. Esta brecha digital abre una oportunidad clara para perfiles ASIR: un espacio poco cubierto donde aportar valor real implementando soluciones profesionales que **modernicen y protejan** a la pequeña empresa sevillana 🛠️💡.

 [⬆️ Volver al índice de apartados](#índice-de-apartados)

---

# **2. Selección de la empresa o contexto de trabajo**


* ### 🏢 Empresa Seleccionada: Soltel Group (Soluciones Tecnológicas S.L.)

Para contextualizar el desarrollo de mi proyecto, he seleccionado como referente a **Soltel Group**, una consultora TIC líder en Andalucía cuya sede central en el **PCT Cartuja** la ubica en el epicentro de la innovación regional 📍. A diferencia de otros entornos, aquí la tecnología es el núcleo del negocio (Core Business), cuentan con una estructura jerárquica muy madura bajo una Dirección Técnica (CTO) organizada en áreas especializadas de **Administración de Sistemas, Ciberseguridad y Cloud & Virtualización** (AWS/Azure) 🏢. Analizar esta empresa es clave porque trabajan bajo estándares de exigencia máxima, cumpliendo normativas como el **Esquema Nacional de Seguridad (ENS)** y la certificación **ISO 27001**, lo que me ofrece un modelo realista de cómo debe planificarse una infraestructura segura, escalable y alineada con las mejores prácticas del mercado 🛡️.

En su operativa diaria, el departamento de sistemas se enfrenta a retos críticos del sector, como la gestión eficiente de costes en la nube pública y la alta rotación de personal técnico ⚠️. Para mitigar estos riesgos y garantizar la continuidad del servicio, Soltel prioriza la **automatización de procesos**, la estandarización y la **monitorización continua** (Observabilidad) ⚙️. La elección de esta compañía como "espejo" es una decisión estratégica: me permite adoptar la perspectiva de una **consultora experta**, aprendiendo sus metodologías profesionales para tener una referencia profesional sólida antes de enfrentarnos al diseño de cualquier solución técnica 🚀💼.

[⬆️ Volver al índice de apartados](#índice-de-apartados)

---

# **3. Identificación de necesidades tecnológicas**

Analizando el entorno real del taller **Triana Motor**, he detectado un nivel de riesgo tecnológico muy elevado: toda la gestión y facturación del negocio depende exclusivamente de un único ordenador de sobremesa local, lo que constituye un **"Punto Único de Fallo"** (SPOF) inaceptable 📉. No existe presencia digital ni copias de seguridad automatizadas, una simple avería de hardware, un robo o un ataque de Ransomware supondría la **pérdida irrecuperable** de años de información de clientes, paralizando por completo la actividad comercial del taller ⚠️.

Para garantizar la supervivencia del negocio, es imprescindible abandonar este modelo local inseguro y migrar hacia una infraestructura **Cloud**. Mi propuesta técnica consiste en un servidor **VPS con Debian** ☁️🐧, desplegar una arquitectura de servicios contenerizados 📦 (**Docker**), separando el Servidor Web 🖥️ (visibilidad) de la Base de Datos 🗄️ (**PostgreSQL/MariaDB**) para proteger la información fuera del local físico. Además, innovar implementando un sistema de observabilidad basado en el Stack TIG (**Telegraf, InfluxDB y Grafana**), configurado para enviar **alertas automáticas ante saturaciones**, permitiendo que el taller pase de la nada tecnológica a contar con un entorno profesional, escalable y vigilado en tiempo real con software **100% Open Source** 📊🚀.

# **4. Oportunidades y viabilidad del proyecto**
# **5. Obligaciones legales y normativas**
# **6. Guion inicial del proyecto**

 


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

- Web Corporativa de Soltel  
    🔗 [Área de Sistemas](https://www.soltel.es/producto/administracion-de-sistemas-e-infraestructuras/)
        
- Esquema Nacional de Seguridad (ENS)  
    🔗 [CCN-CERT](https://ens.ccn.cni.es/es/formacion)
