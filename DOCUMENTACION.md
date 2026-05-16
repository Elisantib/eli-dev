# Documentación Técnica – Portafolio Personal 3D

# Descripción del Proyecto

## Nombre del proyecto
Portafolio Personal 3D

## Tipo de proyecto
Aplicación web estática frontend.

## Objetivo
Desarrollar un portafolio web personal que permita presentar perfil profesional, proyectos, habilidades técnicas y medios de contacto, incorporando elementos interactivos en 3D como diferenciador visual y técnico.

## Objetivos principales

- Construir un proyecto real para portafolio profesional.
- Fortalecer conocimientos en desarrollo frontend.
- Aprender integración de gráficos 3D en entornos web.
- Integrar assets 3D dentro de una aplicación web.
- Crear una base técnica escalable para proyectos futuros.

---

# Alcance Inicial (MVP)

## Funcionalidades incluidas

### Secciones principales

- Inicio
- Sobre mí
- Proyectos
- Habilidades / Stack tecnológico
- Contacto

### Funcionalidades interactivas

- Integración de escena 3D
- Objeto 3D interactivo
- Rotación automática
- Interacción con mouse (hover / click)
- Movimiento básico de cámara
- Animaciones visuales simples
- Transiciones suaves

---

# Arquitectura

## Arquitectura inicial

```text
Navegador
   ↓
HTML / CSS / JavaScript
   ↓
Three.js
   ↓
WebGL
   ↓
Assets 3D (.glb / .gltf)
```

## Tipo de arquitectura
Arquitectura frontend estática.

## Consideraciones

Esta primera versión **no contempla**:

- Backend
- API
- Base de datos
- Autenticación
- Persistencia de datos
- Panel administrativo

### Motivo
El objetivo inicial es mantener una arquitectura simple, enfocada en aprendizaje, velocidad de implementación y facilidad de despliegue.

---

# Stack Tecnológico

# Frontend

## HTML5

Responsable de la estructura semántica del sitio.

### Uso

- Layout general
- Navegación
- Estructura de contenido
- Contenedor del canvas 3D

---

## CSS3

Responsable del diseño visual y comportamiento responsive.

### Uso

- Diseño visual
- Tipografía
- Distribución de componentes
- Responsive design
- Transiciones
- Animaciones complementarias

---

## JavaScript (Vanilla JS)

Lenguaje principal de desarrollo.

### Uso

- Manipulación del DOM
- Manejo de eventos
- Interactividad general
- Integración con Three.js
- Control de animaciones

### Motivo de elección

Se prioriza JavaScript puro para:

- fortalecer fundamentos frontend
- evitar complejidad inicial de frameworks
- facilitar comprensión de arquitectura base
- simplificar debugging
- generar base sólida para futuros proyectos

---

# Motor 3D

## Three.js

Librería JavaScript para renderizado 3D en navegador utilizando WebGL.

## Responsabilidades

- Creación de escena 3D
- Manejo de cámara
- Renderizado
- Iluminación
- Materiales
- Renderizado de meshes
- Animaciones
- Interacciones con objetos
- Carga de modelos 3D

## Casos de uso dentro del proyecto

- Elemento visual principal del portafolio
- Animaciones interactivas
- Diferenciador visual moderno

---

# Modelado 3D

## Blender

Software de modelado 3D utilizado para crear assets personalizados.

## Uso previsto

- Creación de modelos
- Aplicación de materiales
- Animaciones simples
- Exportación optimizada para web

## Formato de exportación

```text
.glb
```

## Motivo de elección

Formato recomendado para web por:

- compatibilidad con Three.js
- peso optimizado
- soporte de materiales
- soporte de animaciones
- facilidad de integración

---

# Herramientas de Desarrollo

## Visual Studio Code

Editor principal del proyecto.

### Uso

- Desarrollo frontend
- Edición de archivos
- Debugging
- Extensiones de productividad

---

## Git

Sistema de control de versiones.

### Uso

- Historial de cambios
- Manejo de ramas
- Recuperación de versiones
- Desarrollo seguro

---

## GitHub

Repositorio remoto del proyecto.

### Uso

- Almacenamiento del código
- Respaldo del proyecto
- Publicación del código
- Integración con despliegue automático

### Tipo de repositorio

```text
Público
```

---

# Hosting / Despliegue

## Opción principal: Netlify

### Tipo
Hosting gratuito para sitios estáticos.

### Beneficios

- gratuito
- integración con GitHub
- despliegue automático
- HTTPS incluido
- dominio temporal incluido
- posibilidad de dominio personalizado

## Flujo de despliegue

```text
Push a GitHub
   ↓
Netlify detecta cambios
   ↓
Build automático
   ↓
Actualización del sitio
```

---

## Alternativa: GitHub Pages

### Beneficios

- gratuito
- simple de configurar
- integrado con GitHub
- ideal para sitios estáticos

### Limitaciones

- menor flexibilidad
- menos opciones de configuración
- menos escalable que Netlify

---

# Estructura Inicial del Proyecto

```text
portafolio-personal/
│
├── index.html
│
├── css/
│   └── styles.css
│
├── js/
│   └── main.js
│
├── assets/
│   ├── images/
│   ├── icons/
│   └── models/
│       └── portfolio-object.glb
│
├── libs/
│   └── three.js
│
└── README.md
```

---

# Backend

## Decisión inicial
No se utilizará backend en la primera versión.

## Razón

El MVP no requiere:

- autenticación
- almacenamiento persistente
- lógica de negocio
- procesamiento de datos
- consumo de API
- base de datos

---

# Escenarios futuros donde sí sería necesario backend

Ejemplos:

- formulario de contacto funcional
- panel administrador
- CMS
- almacenamiento de datos
- autenticación
- chatbot
- integración con IA
- dashboard dinámico

## Stack backend futuro posible

```text
Node.js
Express / NestJS
PostgreSQL
REST API
```

---

# Roadmap de Aprendizaje

## Fase 1 — Fundamentos Frontend

### Enfoque

- HTML
- CSS
- JavaScript
- estructura del sitio
- responsive design

### Entregable

Portafolio estático funcional.

---

## Fase 2 — Integración Three.js

### Enfoque

- escena
- cámara
- iluminación
- render loop
- interacción

### Entregable

Escena 3D funcional.

---

## Fase 3 — Integración de modelos externos

### Enfoque

- carga de modelos `.glb`
- optimización
- animaciones básicas

### Entregable

Modelo 3D integrado.

---

## Fase 4 — Blender

### Enfoque

- modelado básico
- materiales
- exportación web

### Entregable

Primer asset 3D propio.

---

# Estrategia de Versionado

## Ramas sugeridas

```text
main
development
feature/layout
feature/three-scene
feature/model-loader
feature/blender-assets
```

---

# Criterios de éxito del MVP

El proyecto será exitoso si:

- está desplegado públicamente
- funciona correctamente en desktop
- funciona correctamente en mobile
- contiene interacción 3D funcional
- posee despliegue automático desde GitHub
- incluye al menos un asset 3D
- puede ser mostrado como portafolio profesional

---

# Evolución futura (v2)

Posibles mejoras:

- migración a framework (React)
- TypeScript
- GSAP
- backend propio
- formulario funcional
- CMS
- asistente IA
- analytics
- dashboard dinámico
- experiencia 3D más compleja
