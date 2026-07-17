<div align="center">

# 🚀 Aplicación BPM para la Automatización de Penalizaciones Logísticas

### Trabajo Fin de Grado | Ingeniería Informática

**Universidad Europea del Atlántico**

**Autora:** Lydia García Rivero

---

Aplicación desarrollada sobre **AuraQuantic** para automatizar la gestión de penalizaciones logísticas mediante **Business Process Management (BPM)** e **Inteligencia Artificial**.

<img src="images/banner.png" alt="Banner del proyecto" width="900"/>

</div>

---

# 📑 Índice

- [🏭 Contexto del proyecto](#-contexto-del-proyecto)
- [🎯 Objetivos](#-objetivos)
- [🛠 Tecnologías utilizadas](#-tecnologías-utilizadas)
- [📚 Marco teórico](#-marco-teórico)
- [📋 Requerimientos](#-requerimientos)
- [🏗 Análisis y diseño](#-análisis-y-diseño)
- [⚙️ Desarrollo de la solución](#️-desarrollo-de-la-solución)
- [📊 Resultados](#-resultados)
- [🚀 Líneas futuras](#-líneas-futuras)

---

# 🏭 Contexto del proyecto

Este proyecto fue desarrollado durante las prácticas curriculares realizadas en **Andros La Serna**, empresa perteneciente al grupo **Andros**, especializada en la fabricación y distribución de productos lácteos y postres refrigerados.

En su actividad diaria, la empresa trabaja con diferentes operadores logísticos encargados del transporte de mercancías. Cuando durante una entrega se detecta una incidencia, el operador envía una **penalización** mediante correo electrónico indicando la información del pedido afectado, el cliente, los productos implicados y el motivo de la incidencia.

Hasta el momento, la gestión de estas penalizaciones se realizaba de forma completamente manual. Los empleados debían revisar cada correo recibido, interpretar su contenido e introducir toda la información en hojas de cálculo para posteriormente realizar el seguimiento de cada incidencia.

Este procedimiento presentaba diferentes inconvenientes:

- Elevado tiempo de gestión.
- Introducción manual de datos.
- Mayor probabilidad de errores.
- Escasa trazabilidad.
- Información distribuida entre distintos sistemas.

Con el objetivo de mejorar este proceso se desarrolló una aplicación basada en **Business Process Management (BPM)** utilizando la plataforma **AuraQuantic**, capaz de automatizar la recepción de correos electrónicos, analizar automáticamente su contenido mediante **Azure AI Document Intelligence** y generar incidencias listas para su gestión.

<p align="center">
<img src="images/andros.png" width="900"/>
</p>

---

# 🎯 Objetivos

## Objetivo general

Desarrollar una aplicación BPM capaz de automatizar la gestión de penalizaciones logísticas, reduciendo el trabajo manual y mejorando la eficiencia del proceso.

## Objetivos específicos

- Automatizar la recepción de correos electrónicos.
- Eliminar la introducción manual de datos.
- Extraer automáticamente la información mediante Inteligencia Artificial.
- Crear incidencias automáticamente.
- Centralizar toda la información en una única aplicación.
- Mejorar la trazabilidad del proceso.
- Reducir el tiempo de gestión.
- Minimizar errores humanos.

---

# 🛠 Tecnologías utilizadas

| Tecnología | Descripción |
|------------|-------------|
| **AuraQuantic** | Plataforma Low-Code para el desarrollo de procesos BPM. |
| **Azure AI Document Intelligence** | Servicio de Inteligencia Artificial para el análisis de documentos. |
| **REST API** | Comunicación entre AuraQuantic y Azure. |
| **Microsoft Azure** | Plataforma cloud utilizada para los servicios de IA. |
| **Business Process Management (BPM)** | Metodología utilizada para modelar y automatizar procesos. |
| **PDF** | Conversión automática de los correos electrónicos para su procesamiento. |

---

# 📚 Marco teórico

## Business Process Management (BPM)

Business Process Management (BPM) es una metodología orientada al análisis, modelado, automatización y mejora continua de procesos empresariales.

En este proyecto constituye la base sobre la que se diseña todo el flujo de gestión de penalizaciones, permitiendo automatizar tareas repetitivas y mejorar la eficiencia del proceso.

<p align="center">
<img src="images/bpm.png" width="700"/>
</p>

---

## AuraQuantic

AuraQuantic es una plataforma **Low-Code** especializada en la automatización de procesos empresariales.

Toda la aplicación desarrollada en este proyecto ha sido implementada utilizando esta plataforma, permitiendo modelar procesos, diseñar formularios, gestionar datos e integrar servicios externos.

Con AuraQuantic se han desarrollado:

- Procesos automáticos.
- Formularios.
- Gestión de incidencias.
- Maestros de clientes y artículos.
- Automatización del flujo completo.

<p align="center">
<img src="images/auraquantic.png" width="750"/>
</p>

---

## Azure AI Document Intelligence

Para automatizar la lectura de los correos electrónicos se ha utilizado **Azure AI Document Intelligence**, un servicio de Microsoft Azure basado en Inteligencia Artificial capaz de analizar documentos y extraer información estructurada.

Tras entrenar el modelo con ejemplos reales de penalizaciones, el sistema es capaz de identificar automáticamente los campos necesarios para crear las incidencias.

<p align="center">
<img src="images/azure-training.png" width="750"/>
</p>

<p align="center">
<img src="images/azure-result.png" width="750"/>
</p>

---

## Automatización de procesos

La solución desarrollada automatiza completamente el flujo inicial de gestión de penalizaciones.

Las principales tareas automatizadas son:

- Recuperación de correos electrónicos.
- Conversión del correo a PDF.
- Envío del documento a Azure.
- Extracción automática de la información.
- Validación de los datos.
- Creación automática de incidencias.

---

# 📋 Requerimientos

## Requerimientos funcionales

- Recuperación automática de correos.
- Procesamiento mediante Inteligencia Artificial.
- Creación automática de incidencias.
- Gestión de estados.
- Asignación de responsables.
- Consulta de incidencias.
- Gestión de clientes.
- Gestión de artículos.

## Requerimientos no funcionales

- Escalabilidad.
- Seguridad.
- Rendimiento.
- Disponibilidad.
- Usabilidad.
- Mantenibilidad.

---

# 🏗 Análisis y diseño

Antes del desarrollo de la aplicación fue necesario analizar el procedimiento utilizado por la empresa para gestionar las penalizaciones logísticas.

Durante esta fase se estudiaron numerosos correos electrónicos enviados por el operador logístico con el objetivo de identificar la información necesaria para automatizar el proceso y diseñar la estructura de datos que posteriormente sería utilizada en AuraQuantic.

El análisis permitió detectar diferentes situaciones, como correos con formatos distintos, campos incompletos o varias incidencias dentro del mismo mensaje, definiendo una solución flexible capaz de adaptarse a todos estos escenarios.

Como resultado de esta fase se elaboraron diferentes diagramas UML para representar la arquitectura y el funcionamiento del sistema:

- Diagrama de contexto.
- Diagrama de casos de uso.
- Diagrama de actividades.
- Diagrama de clases.
- Diagrama de objetos.
- Diagrama de secuencia.

<p align="center">
<img src="images/contexto.png" width="850"/>
</p>

---

---

# ⚙️ Desarrollo de la solución

Tras finalizar la fase de análisis y diseño, se desarrolló una aplicación sobre **AuraQuantic** capaz de automatizar el proceso completo de gestión de penalizaciones logísticas.

La solución está formada por tres procesos principales que trabajan de forma coordinada para recibir los correos electrónicos, analizar automáticamente su contenido y generar incidencias dentro de la aplicación.

## Arquitectura general

```mermaid
flowchart LR

A[📧 Correo recibido] --> B[Proceso 21]
B --> C[Proceso 22]
C --> D[Azure AI Document Intelligence]
D --> E[Datos extraídos]
E --> F[Proceso 23]
F --> G[Incidencia creada]
G --> H[Gestión por el usuario]
```

---

# 📧 Proceso 21 - Recuperación de correos electrónicos

El primer proceso desarrollado tiene como objetivo recuperar automáticamente los correos electrónicos enviados por el operador logístico.

Para ello, AuraQuantic establece una conexión con el buzón corporativo donde se reciben las penalizaciones y obtiene todos aquellos mensajes pendientes de procesamiento.

Una vez recuperados, cada correo es preparado para su posterior tratamiento por el siguiente proceso.

### Funciones principales

- Recuperación automática de correos.
- Conexión con el buzón corporativo.
- Control de errores.
- Registro de la ejecución.
- Envío del correo al Proceso 22.

<p align="center">
<img src="images/proceso21.png" width="900"/>
</p>

---

# 🤖 Proceso 22 - Extracción automática de información

El segundo proceso es el encargado de interpretar automáticamente el contenido de cada correo electrónico.

En primer lugar, el correo recibido se convierte a formato PDF para facilitar su análisis. Posteriormente, dicho documento se envía mediante una API REST a **Azure AI Document Intelligence**, que procesa el contenido utilizando un modelo previamente entrenado.

Una vez finalizado el análisis, Azure devuelve la información estructurada al proceso de AuraQuantic, donde es validada antes de continuar con la creación de la incidencia.

### Flujo del proceso

```mermaid
flowchart LR

A[Correo electrónico]
-->B[Conversión a PDF]
-->C[Azure AI Document Intelligence]
-->D[Extracción de datos]
-->E[Validación]
-->F[Proceso 23]
```

<p align="center">
<img src="images/proceso22.png" width="900"/>
</p>

## Conversión automática a PDF

Antes del análisis, el correo electrónico se transforma automáticamente en un documento PDF.

<p align="center">
<img src="images/pdf.png" width="700"/>
</p>

---

## Azure AI Document Intelligence

Para la extracción de la información se entrenó un modelo de Inteligencia Artificial capaz de reconocer automáticamente los diferentes campos presentes en las penalizaciones.

<p align="center">
<img src="images/azure-training.png" width="750"/>
</p>

Una vez procesado el documento, Azure devuelve todos los datos estructurados.

<p align="center">
<img src="images/azure-result.png" width="750"/>
</p>

### Campos extraídos

La solución identifica automáticamente información como:

- Número de ticket.
- Fecha.
- Albarán.
- Cliente.
- Destinatario.
- Palés.
- Bultos.
- Peso.
- Temperatura.
- Tipo de anomalía.
- Motivo de la penalización.
- Información del producto.

En total se extraen **17 campos** automáticamente.

---

# 💾 Proceso 23 - Creación automática de incidencias

Una vez obtenida la información, el tercer proceso transforma los datos al formato interno de la aplicación y crea automáticamente una nueva incidencia.

Durante este proceso también se realizan diferentes validaciones para comprobar la integridad de la información antes de almacenarla definitivamente.

### Funciones principales

- Recepción de los datos extraídos.
- Conversión al modelo de datos.
- Generación del identificador.
- Validación.
- Almacenamiento.
- Gestión de errores.

<p align="center">
<img src="images/proceso23.png" width="900"/>
</p>

---

# 🖥️ Gestión de incidencias

Una vez creada, la incidencia queda registrada automáticamente dentro de la aplicación.

Desde esta pantalla los usuarios pueden:

- Consultar todas las incidencias.
- Asignar responsables.
- Actualizar el estado.
- Revisar la información extraída.
- Añadir observaciones.

<p align="center">
<img src="images/incidencias.png" width="900"/>
</p>

Cada incidencia dispone además de una vista detallada donde se muestra toda la información obtenida durante el procesamiento.

<p align="center">
<img src="images/detalle-incidencia.png" width="850"/>
</p>

---

# 📚 Gestión de maestros

La aplicación incorpora dos módulos adicionales que permiten consultar información relacionada con las incidencias.

## Maestro de artículos

Permite consultar toda la información referente a los productos registrados en el sistema.

<p align="center">
<img src="images/maestro-articulos.png" width="850"/>
</p>

---

## Maestro de clientes

Permite acceder a la información de todos los clientes registrados.

<p align="center">
<img src="images/maestro-clientes.png" width="850"/>
</p>

---

# 📊 Resultados

La solución desarrollada ha permitido automatizar completamente la fase inicial del proceso de gestión de penalizaciones.

| Indicador | Resultado |
|-----------|-----------|
| Correos procesados automáticamente | ✅ |
| Extracción automática de datos | ✅ |
| Creación automática de incidencias | ✅ |
| Campos identificados | **17** |
| Centralización de la información | ✅ |
| Reducción del trabajo manual | ✅ |

Los resultados obtenidos muestran una mejora significativa en la eficiencia del proceso, reduciendo el tiempo dedicado a tareas repetitivas y mejorando la trazabilidad de las incidencias.

---

# 🚀 Líneas futuras

Aunque la aplicación cumple con los objetivos definidos inicialmente, existen diferentes líneas de evolución que permitirían ampliar sus funcionalidades:

- Integración con el ERP **Agena**.
- Integración con **Telifrai**.
- Automatización del proceso completo de validación de penalizaciones.
- Incorporación de cuadros de mando con indicadores.
- Generación automática de informes.
- Nuevos procesos BPM para otras áreas de la empresa.

---

<div align="center">

## 👩‍💻 Autora

**Lydia García Rivero**

Grado en Ingeniería Informática

Universidad Europea del Atlántico

---

⭐ Gracias por visitar este proyecto.

</div>
