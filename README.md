# grachi 🧿

Colección de pequeñas webs estáticas, hechas con cariño.
Monorepo: cada carpeta es un producto/mini-proyecto independiente y autocontenido (HTML/CSS/JS, sin build).

## Proyectos

| Proyecto | Descripción | Demo local |
|----------|-------------|------------|
| [`cartas/`](./cartas) | Sobres digitales "Ábrelo cuando…" estilo nazar (ojo turco). | `cartas/index.html` |
| [`audiencias-virtuales/`](./audiencias-virtuales) | Cinco mini-juegos sueltos, tema "Tribunal de la Distancia"; cada uno reparte un premio al azar (regalo real o promesa) de un pozo compartido. | `audiencias-virtuales/*.html` |

## Estructura

```
grachi/
├── README.md
├── cartas/
│   ├── index.html      ← abre directo en el navegador
│   └── README.md
└── audiencias-virtuales/
    ├── ruleta_audiencias.html
    ├── sello_confidencial.html
    ├── examen_barra_amor.html
    ├── reconstruye_pruebas.html
    ├── recurso_inapelable.html
    └── README.md
```

Cada proyecto vive en su propia carpeta y es 100 % estático: se puede abrir con doble clic o servir desde GitHub Pages / Netlify / Vercel sin configuración.

## Desplegar en GitHub Pages

1. *Settings → Pages → Source: Deploy from a branch* (`main`, carpeta `/root`).
2. Cada proyecto queda disponible en `https://<usuario>.github.io/grachi/cartas/`.
