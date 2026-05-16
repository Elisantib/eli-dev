# Portafolio Personal 3D

Portafolio web personal con elementos interactivos en 3D, construido con HTML, CSS, JavaScript y Three.js.

> Para la documentación técnica completa (arquitectura, roadmap, decisiones técnicas), ver [DOCUMENTACION.md](DOCUMENTACION.md).

---

## Tabla de contenidos

- [Descripción](#descripción)
- [Características](#características)
- [Stack tecnológico](#stack-tecnológico)
- [Estructura del proyecto](#estructura-del-proyecto)
- [Requisitos previos](#requisitos-previos)
- [Instalación](#instalación)
- [Uso](#uso)
- [Despliegue](#despliegue)
- [Roadmap](#roadmap)
- [Contribución](#contribución)
- [Licencia](#licencia)
- [Contacto](#contacto)

---

## Descripción

Sitio web estático que presenta perfil profesional, proyectos, habilidades y medios de contacto. Incorpora una escena 3D interactiva como diferenciador visual, renderizada con Three.js sobre WebGL.

---

## Características

- Secciones: Inicio, Sobre mí, Proyectos, Habilidades, Contacto.
- Escena 3D integrada en el navegador.
- Objeto 3D interactivo (rotación automática, hover y click).
- Movimiento básico de cámara.
- Diseño responsive (desktop y mobile).
- Transiciones y animaciones suaves.
- Despliegue automático desde GitHub.

---

## Stack tecnológico

| Categoría    | Tecnología              |
|--------------|-------------------------|
| Estructura   | HTML5                   |
| Estilos      | CSS3                    |
| Lógica       | JavaScript (Vanilla JS) |
| Motor 3D     | Three.js (WebGL)        |
| Modelado 3D  | Blender (`.glb`)        |
| Versionado   | Git + GitHub            |
| Hosting      | Netlify (alt. GitHub Pages) |
| Editor       | Visual Studio Code      |

---

## Estructura del proyecto

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
├── README.md
└── DOCUMENTACION.md
```

---

## Requisitos previos

- Navegador moderno con soporte WebGL (Chrome, Firefox, Edge, Safari).
- Git instalado (para clonar el repositorio).
- Opcional: un servidor local (Live Server, `http-server`, etc.) para evitar errores de CORS al cargar modelos `.glb`.

---

## Instalación

1. Clonar el repositorio:

   ```bash
   git clone https://github.com/<usuario>/portafolio-personal.git
   cd portafolio-personal
   ```

2. (Opcional) Iniciar un servidor local:

   - Con la extensión **Live Server** de VS Code: clic derecho sobre `index.html` → *Open with Live Server*.
   - O con Node.js:

     ```bash
     npx http-server .
     ```

3. Abrir en el navegador:

   ```text
   http://localhost:8080
   ```

---

## Uso

- Navegar entre secciones desde el menú principal.
- Interactuar con el objeto 3D mediante mouse (hover y click).
- Observar la rotación automática y las animaciones de cámara.

No se requiere build ni instalación de dependencias: es un sitio estático.

---

## Despliegue

### Netlify (recomendado)

1. Iniciar sesión en [Netlify](https://www.netlify.com/) con la cuenta de GitHub.
2. *Add new site → Import an existing project → GitHub*.
3. Seleccionar el repositorio.
4. Build command: *(vacío)* — Publish directory: `/`.
5. Cada `push` a `main` ejecuta un despliegue automático.

### GitHub Pages (alternativa)

1. *Settings → Pages*.
2. Source: rama `main`, carpeta `/root`.
3. Guardar — el sitio quedará disponible en `https://<usuario>.github.io/portafolio-personal/`.

---

## Roadmap

- **Fase 1** — Fundamentos frontend (HTML, CSS, JS, responsive).
- **Fase 2** — Integración de Three.js (escena, cámara, iluminación).
- **Fase 3** — Carga de modelos `.glb` y animaciones.
- **Fase 4** — Modelado propio en Blender.

Mejoras previstas para la **v2**: migración a React, TypeScript, GSAP, backend propio, formulario funcional, CMS, integración de IA, analytics. Detalle en [DOCUMENTACION.md](DOCUMENTACION.md#evolución-futura-v2).

---

## Contribución

Este es un proyecto personal de aprendizaje, pero las sugerencias son bienvenidas:

1. Hacer un fork del repositorio.
2. Crear una rama: `git checkout -b feature/mi-mejora`.
3. Commit de los cambios: `git commit -m "feat: descripción"`.
4. Push a la rama: `git push origin feature/mi-mejora`.
5. Abrir un Pull Request.

### Ramas del proyecto

```text
main
development
feature/layout
feature/three-scene
feature/model-loader
feature/blender-assets
```

---

## Licencia

Este proyecto se distribuye bajo licencia **MIT**. Ver el archivo `LICENSE` para más información.

---

## Contacto

- **Autora:** Elisa Santibáñez
- **Email:** elisa.santibanez@geti.cl
- **GitHub:** [@elisantidev](https://github.com/elisantidev)
