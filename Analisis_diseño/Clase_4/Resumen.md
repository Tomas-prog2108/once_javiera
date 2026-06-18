# Documentación de Requerimientos

## ¿Qué es la Documentación de Requerimientos?

La documentación de requerimientos consiste en registrar de forma clara, organizada y verificable las necesidades y expectativas del sistema. Sirve como referencia para todos los involucrados durante el ciclo de vida del proyecto.

---

## Funciones de la Documentación de Requerimientos

### Acuerdo
- Actúa como un contrato entre el cliente y el equipo de desarrollo.
- Define qué se espera que entregue el sistema.

### Guía
- Orienta a los desarrolladores sobre qué construir.
- Reduce ambigüedades durante la implementación.

### Verificación
- Permite a los testers comprobar que el sistema cumple lo prometido.
- Sirve como base para diseñar casos de prueba.

### Conocimiento
- Conserva la información y decisiones del proyecto.
- Funciona como memoria organizacional, incluso cuando cambian los integrantes del equipo.

### Legal
- Puede utilizarse como evidencia en auditorías, contratos o disputas.
- Documenta formalmente los compromisos adquiridos.

---

## Estándar IEEE 830

El **IEEE 830** es un estándar internacional desarrollado por el **Institute of Electrical and Electronics Engineers (IEEE)** que establece recomendaciones para elaborar una **Especificación de Requerimientos de Software (SRS - Software Requirements Specification)**.

Su objetivo es garantizar que los requerimientos sean claros, completos, consistentes y verificables.

---

## Estructura del Documento IEEE 830

### 1. Introducción

Presenta el contexto general del documento.

#### Contenido
- Introducción
- Alcance
- Definiciones, acrónimos y abreviaturas
- Referencias
- Visión general del documento

---

### 2. Descripción General

Proporciona una visión global del sistema antes de detallar los requerimientos.

#### Componentes

- **Perspectiva del producto**
  - Relación del sistema con otros productos o sistemas.

- **Funciones del producto**
  - Capacidades principales que ofrecerá el software.

- **Características del usuario**
  - Perfil de los usuarios que utilizarán el sistema.

- **Restricciones**
  - Limitaciones técnicas, legales o de negocio.

- **Suposiciones y dependencias**
  - Factores externos de los que depende el sistema.

---

### 3. Requisitos Específicos

Describe de manera detallada los requerimientos del sistema.

#### Incluye

- Requerimientos funcionales
- Requerimientos no funcionales
- Interfaces externas
- Casos de uso

---

### 4. Apéndices

Información complementaria que facilita la comprensión del documento.

#### Ejemplos

- Diagramas adicionales
- Glosario extendido
- Bocetos de pantallas
- Tablas de trazabilidad

---

## Casos de Uso

Un **caso de uso** es una descripción narrativa de la interacción entre un usuario y el sistema para alcanzar un objetivo específico.

Permite representar cómo los actores utilizan el sistema y ayuda a comprender los requerimientos funcionales desde la perspectiva del usuario.

---

## Plantilla de Caso de Uso

Un caso de uso suele documentarse mediante la siguiente estructura:

| Campo | Descripción |
|---------|-------------|
| **ID** | Identificador único del caso de uso. |
| **Nombre** | Nombre representativo del proceso. |
| **Actor(es) principal(es)** | Usuario o entidad que inicia la interacción. |
| **Descripción breve** | Resumen del objetivo del caso de uso. |
| **Precondiciones** | Condiciones que deben cumplirse antes de iniciar. |
| **Postcondiciones** | Estado esperado al finalizar exitosamente. |
| **Flujo principal** | Secuencia normal de pasos para completar el objetivo. |
| **Flujos alternos** | Variaciones o caminos opcionales del proceso. |
| **Excepciones** | Situaciones de error o fallo. |
| **Reglas de negocio** | Restricciones y políticas aplicables. |
| **Frecuencia de uso** | Qué tan seguido se ejecuta el proceso. |
| **Prioridad** | Nivel de importancia para el negocio o proyecto. |
