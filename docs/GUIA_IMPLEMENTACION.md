# 🚀 Guía Completa: TuCompraOK en GitHub Pages

## 📋 Tabla de Contenidos
1. [Estructura del Proyecto](#estructura-del-proyecto)
2. [Configuración en GitHub Pages](#configuración-en-github-pages)
3. [Cómo Agregar Productos](#cómo-agregar-productos)
4. [Conectar Dominio](#conectar-dominio)
5. [Optimización SEO](#optimización-seo)
6. [Tips de Marketing](#tips-de-marketing)

---

## 📁 Estructura del Proyecto

```
tucompraok.github.io/
│
├── index.html                          # Landing principal (galería)
├── README.md
├── sitemap.xml                         # Para SEO
│
├── /productos/
│   ├── uniclean-oxigeno-activo/
│   │   └── index.html                  # Landing del producto
│   ├── smartwatch-pro/
│   │   └── index.html
│   └── almohada-ergonomica/
│       └── index.html
│
├── /assets/
│   ├── /css/
│   │   └── styles.css                  # Estilos compartidos (opcional)
│   ├── /img/
│   │   ├── uniclean.png
│   │   ├── smartwatch.png
│   │   └── ...otros productos
│   └── /js/
│       └── main.js                     # Scripts compartidos
│
└── /docs/
    └── PLANTILLA_PRODUCTO.html         # Plantilla para copiar
```

---

## ⚙️ Configuración en GitHub Pages

### Paso 1: Crear un Repositorio en GitHub
1. Ve a https://github.com/new
2. **Nombre del repositorio:** `tucompraok.github.io`
3. Marca "Public"
4. Crea el repositorio

### Paso 2: Subir los Archivos
#### Opción A: Con Git (Recomendado)
```bash
# Clonar el repositorio
git clone https://github.com/tu-usuario/tucompraok.github.io.git
cd tucompraok.github.io

# Crear la estructura
mkdir -p productos/uniclean-oxigeno-activo
mkdir -p assets/img assets/css assets/js

# Copiar tus archivos HTML
cp /ruta/tucompraok-index.html index.html
cp /ruta/tucompraok-producto-template.html productos/uniclean-oxigeno-activo/index.html

# Subir a GitHub
git add .
git commit -m "Initial commit: TuCompraOK landing pages"
git push origin main
```

#### Opción B: Interfaz Web (Sin Git)
1. En tu repositorio, ve a "Add file" → "Upload files"
2. Arrastra tu `index.html`
3. Crea carpetas manualmente y sube archivos

### Paso 3: Activar GitHub Pages
1. Ve a Settings del repositorio
2. Busca "Pages" en el menú izquierdo
3. Bajo "Build and deployment":
   - Source: "Deploy from a branch"
   - Branch: "main" / "root"
4. Guarda
5. Tu sitio estará en: `https://tucompraok.github.io`

---

## ➕ Cómo Agregar Productos

### Template para Nuevo Producto

Usa `tucompraok-producto-template.html` como base y modifica:

```html
<!-- 1. Cambiar el título de la página -->
<title>NombreProducto | TuCompraOK</title>

<!-- 2. Cambiar la categoría -->
<span class="category-tag">🏷️ Tu Categoría</span>

<!-- 3. Cambiar título principal -->
<h1 class="product-title">Tu titular atractivo</h1>

<!-- 4. Cambiar el enlace de Mercado Libre -->
<a href="https://mercadolibre.com.ar/..." target="_blank" class="btn btn-primary">

<!-- 5. Actualizar las características principales -->
<ul>
    <li><strong>Característica 1</strong> - Descripción</li>
    <li><strong>Característica 2</strong> - Descripción</li>
</ul>

<!-- 6. Cambiar los emojis del ícono -->
<div class="product-image">🔧</div>  <!-- Cambiar este emoji -->

<!-- 7. Actualizar especificaciones -->
<div class="spec-item">
    <div class="spec-label">Marca</div>
    <div class="spec-value">Tu Marca</div>
</div>
```

### Ejemplo Práctico: Producto Nuevo

**Estructura de carpetas:**
```
/productos/
  /mi-nuevo-producto/
    index.html
    producto.jpg (opcional)
```

**Crear el archivo `index.html` con:**
1. Copiar plantilla
2. Reemplazar datos
3. Guardar en `/productos/mi-nuevo-producto/index.html`
4. GitHub actualizará automáticamente (5-10 segundos)

---

## 🌐 Conectar tu Dominio tucompraok.online

### Opción 1: Con Namecheap, GoDaddy, etc.

1. En GitHub (Settings → Pages):
   - Custom domain: `tucompraok.online`
   - Haz clic "Save"

2. En tu registrador de dominio (Namecheap, GoDaddy):
   - Ve a DNS Settings
   - Añade estos registros:
     ```
     CNAME: www.tucompraok.online → tucompraok.github.io
     A: tucompraok.online → 185.199.108.153
                          → 185.199.109.153
                          → 185.199.110.153
                          → 185.199.111.153
     ```

3. Espera 24-48 horas a que se propague

### Opción 2: Sin registrador (Redirigir)
Si ya tienes tucompraok.online en Shopify:
- Puede redirigirse a: `https://tucompraok.github.io`
- Mantener la URL original no es posible sin control de DNS

---

## 🔍 Optimización SEO

### 1. Agregar Sitemap
Crea `/sitemap.xml`:
```xml
<?xml version="1.0" encoding="UTF-8"?>
<urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
  <url>
    <loc>https://tucompraok.online</loc>
    <lastmod>2025-01-15</lastmod>
    <priority>1.0</priority>
  </url>
  <url>
    <loc>https://tucompraok.online/productos/uniclean-oxigeno-activo/</loc>
    <lastmod>2025-01-15</lastmod>
    <priority>0.8</priority>
  </url>
</urlset>
```

### 2. Meta Tags Importantes
Incluye en cada `<head>`:
```html
<meta name="description" content="Descripción breve del producto - 160 caracteres">
<meta name="keywords" content="oxígeno activo, limpieza, desincrustante">
<meta property="og:title" content="Título para redes sociales">
<meta property="og:description" content="Descripción para compartir">
<meta property="og:image" content="https://tucompraok.online/assets/img/producto.jpg">
```

### 3. Velocidad de Página
- Optimiza imágenes con TinyPNG.com
- Usa format WebP para mejor compresión
- Minimiza CSS/JS si es posible

### 4. Registrarse en Google Search Console
1. Ve a https://search.google.com/search-console
2. Verifica tu dominio
3. Sube el sitemap.xml
4. Espera indexación (1-2 semanas)

---

## 📱 Tips de Marketing para Meta Ads

### Estructura de Campanillas de Ads

**Elemento 1: Landing Principal**
- URL: `https://tucompraok.online`
- Objetivo: Conciencia de marca
- Audiencia: Amplia, intereses en compra online

**Elemento 2: Producto Específico**
- URL: `https://tucompraok.online/productos/uniclean-oxigeno-activo/`
- Objetivo: Conversión (clic a Mercado Libre)
- Audiencia: Segmentada por interés (ej: "limpieza hogar", "aseo")

### Texto de Anuncio Recomendado

```
Titular:
"Oxígeno Activo que Recupera tu Ropa"

Descripción:
"Elimina manchas difíciles sin dañar telas. 1KG rendidor. 
Compra segura en Mercado Libre. Envío a todo Chile."

CTA: "Comprar Ahora"
```

### Pixel de Facebook
Agregar a cada página:
```html
<script async defer crossorigin="anonymous" 
src="https://connect.facebook.net/es_LA/sdk.js#xfbml=1&version=v18.0" 
nonce="XXXXXXXX"></script>
```

---

## 🔧 Mantenimiento Regular

### Actualizar Productos
1. Editar HTML directamente en GitHub
2. Cambios se reflejan al guardar (5-10 seg)
3. No requiere re-deploy

### Monitorear Rendimiento
1. Google Analytics:
   - Agregar código UA- a cada página
   - Rastrear clics a Mercado Libre

2. Mercado Libre:
   - Ver cuántos clics vinieron desde tu landing
   - Ajustar títulos/descripciones según engagement

### Actualizar Enlaces
Cada que subas un nuevo producto a Mercado Libre:
1. Copia el enlace
2. Edita el HTML del producto
3. Reemplaza `href="https://mercadolibre.com.ar/..."`
4. Guarda

---

## ⚡ Checklist Inicial

- [ ] Crear repositorio `tucompraok.github.io`
- [ ] Subir `index.html` (landing principal)
- [ ] Crear carpeta `/productos/primer-producto/`
- [ ] Subir primer landing individual
- [ ] Activar GitHub Pages
- [ ] Conectar dominio tucompraok.online
- [ ] Crear sitemap.xml
- [ ] Registrar en Google Search Console
- [ ] Configurar Meta Pixel
- [ ] Crear primeras campañas en Meta Ads

---

## 📞 Soporte

**Problemas comunes:**

| Problema | Solución |
|----------|----------|
| Sitio no aparece | Espera 5-10 min, recarga caché (Ctrl+Shift+R) |
| Dominio no funciona | Verifica DNS, espera 48h |
| Cambios no se ven | Limpia caché del navegador |
| Imagen no carga | Verifica ruta relativa: `/assets/img/nombre.jpg` |

---

**Hecho para crecer. Mantén esto simple, rápido y enfocado en conversión.** 🚀
