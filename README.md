# Portafolio Personal 3D

> Para la documentación técnica completa (arquitectura, roadmap, decisiones técnicas), ver [DOCUMENTACION.md](DOCUMENTACION.md).

---

## Tabla de contenidos

- [Descripción](#descripción)
- [Características](#características)
- [Stack tecnológico](#stack-tecnológico)
- [Estructura del proyecto](#estructura-del-proyecto)
- [Requisitos previos](#requisitos-previos)
- [Uso](#uso)
- [Despliegue](#despliegue)
- [Roadmap](#roadmap)
- [Contribución](#contribución)
- [Contacto](#contacto)

---

## Descripción

Este proyecto corresponde a mi portafolio personal, desarrollado como un sitio web estático diseñado para presentar mi perfil profesional y personal, experiencia, proyectos, habilidades técnicas y medios de contacto.

Más que solo un portafolio, este proyecto representa parte de mi camino como desarrolladora, reuniendo lo esencial de una profesional con casi 2 años de experiencia en desarrollo de software, además de reflejar mi interés por seguir aprendiendo, construir proyectos propios y fortalecer continuamente mis habilidades técnicas.

También es un proyecto realizado con mucho cariño y dedicación, como una forma de agradecer a todas las personas que han sido parte de mi proceso de aprendizaje hasta hoy: amigos, profesores, compañeros de trabajo y familia, quienes de una u otra forma han contribuido a mi crecimiento profesional y personal.

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
- Git instalado.
- Opcional: un servidor local (Live Server, `http-server`, etc.) para evitar errores de CORS al cargar assets.

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
- **Fase 3** — Carga de modelos e integración de animaciones.

Mejoras previstas para la **v2**: migración a React, TypeScript, GSAP, backend propio, formulario funcional, CMS, integración de IA, analytics. Detalle en [DOCUMENTACION.md](DOCUMENTACION.md).

---

## Contribución

Este es un proyecto personal de aprendizaje, pero las sugerencias son bienvenidas:

1. Hacer un fork del repositorio.
2. Crear una rama: `git checkout -b feature/mi-mejora`.
3. Commit de los cambios: `git commit -m "feat: descripción"`.
4. Push a la rama: `git push origin feature/mi-mejora`.
5. Abrir un Pull Request.

---

## Contacto

- **Email:** elisa.asp94@gmail.com
- **GitHub:** [@Elisantib](https://github.com/Elisantib)
