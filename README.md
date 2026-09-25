# 🐺 White Lab

Proyecto web desarrollado para la competencia. Incluye estructura modular con carpetas separadas para estilos, scripts, datos y recursos visuales, además de una carpeta de documentación.

---

## 📁 Estructura del proyecto

```
rem/
├── .venv/              # Entorno virtual de Python (NO subir a Git)
├── docs/               # Documentación e investigación del proyecto
├── src/
│   ├── assets/         # Recursos estáticos del sitio
│   │   ├── icons/      # Iconos en formato SVG, PNG o ICO
│   │   └── img/        # Imágenes, fotos y gráficos del proyecto
│   ├── css/            # Hojas de estilo (styles.css, reset.css, etc.)
│   ├── data/           # Archivos de datos (JSON, CSV, XML)
│   ├── js/             # Scripts JavaScript (lógica del sitio)
│   └── index.html      # Página principal del proyecto
├── README.md           # Este archivo
└── .gitignore          # Archivos y carpetas ignoradas por Git
```

---

## 📂 Descripción de cada carpeta

### `.venv/`
Entorno virtual de Python. Contiene las librerías instaladas para este proyecto. **No se sube a Git** (debe estar en `.gitignore`).

### `docs/`
Documentación del proyecto: investigación, apuntes, referencias, diagramas y cualquier material teórico. Puede contener archivos `.md`, `.pdf`, imágenes y enlaces.
- `docs/README.md` → índice de la documentación (opcional)
- `docs/pdfs/` → artículos y reportes descargados
- `docs/imagenes/` → diagramas y capturas usadas en los documentos

### `src/`
Carpeta raíz del código fuente del sitio web. Todo lo que el navegador necesita vive aquí.

### `src/assets/`
Recursos estáticos reutilizables.

- **`assets/icons/`** → Iconos del sitio (favicon, iconos de navegación, botones). Formatos recomendados: `.svg`, `.png`, `.ico`.
- **`assets/img/`** → Imágenes generales: fotos, ilustraciones, logotipos, banners.

### `src/css/`
Hojas de estilo del proyecto. Aquí van todos los archivos `.css`. Se recomienda separar por responsabilidad:
- `reset.css` → normalización de estilos del navegador
- `styles.css` → estilos principales
- `responsive.css` → media queries

### `src/data/`
Archivos de datos que se cargan dinámicamente. Ejemplos: `productos.json`, `usuarios.json`, `config.json`. Útil si el sitio consume datos sin backend.

### `src/js/`
Scripts JavaScript que dan interactividad al sitio. Se recomienda separar por módulos:
- `main.js` → inicialización
- `api.js` → llamadas a datos
- `ui.js` → manipulación del DOM

### `src/index.html`
Página principal del sitio. Punto de entrada del proyecto web.

---

## 🚀 Cómo ejecutarlo

### Requisitos
- Python 3.10 o superior
- Un navegador web moderno

### Pasos

```bash
# 1. Clonar el repositorio
git clone https://github.com/Lau1216/human-firewall.git
cd rem

# 2. Crear entorno virtual (si no existe)
python -m venv .venv

# 3. Activar entorno virtual
# Windows:
.venv\Scripts\activate
# Linux/Mac:
source .venv/bin/activate

# 4. Abrir el sitio
# Opción A: abrir src/index.html directamente en el navegador
# Opción B: usar un servidor local
python -m http.server 8000 --directory src
# Luego ir a http://localhost:8000
```

---

## ✏️ Convenciones de trabajo

- **Nombres de archivos**: `kebab-case` para CSS/HTML (`mi-archivo.css`), `camelCase` para JS (`miFuncion.js`).
- **Imágenes**: guardar en `assets/img/` con nombres descriptivos (`logo-principal.png`, no `img1.png`).
- **Documentación**: todo lo teórico va en `docs/`, separado del código.
- **Commits**: mensajes claros en español, ej: `"Añadir estilos del header"`.

---

## 👥 Autores

- **Lau1216**

---

## ⚠️ Notas

- El `.venv/` está en `.gitignore` y **no debe subirse**.
- Antes de hacer `git push`, verifica con `git status` que solo subes lo que quieres.