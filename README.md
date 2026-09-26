# 🛒 TuCompraOK - Tienda Online Premium

Tienda online gratuita en GitHub Pages con landing principal + landings individuales de productos. Todo enlazado a Mercado Libre para máxima conversión con gastos mínimos.

**Live:** https://tucompraok.online  
**Repo:** https://github.com/tu-usuario/tucompraok.github.io

---

## ✨ Características

✅ **Landing principal** con galería de productos filtrable  
✅ **Landing individual** por producto (estilo 3pod)  
✅ **Responsive** en móvil, tablet y desktop  
✅ **Gratuito** - Hosting en GitHub Pages  
✅ **Rápido** - Carga en <1 segundo  
✅ **SEO-friendly** - Optimizado para buscadores  
✅ **Directo a Mercado Libre** - Botones enlazados  

---

## 🚀 Inicio Rápido

### 1. Clonar este repositorio
```bash
git clone https://github.com/tu-usuario/tucompraok.github.io.git
cd tucompraok.github.io
```

### 2. Estructura de carpetas
```
├── index.html                    # Landing principal
├── sitemap.xml                   # Para SEO
├── README.md
│
├── /productos/
│   ├── uniclean-oxigeno-activo/
│   │   └── index.html
│   ├── smartwatch-pro/
│   │   └── index.html
│   └── [agregar más productos]
│
└── /assets/
    ├── /img/
    │   ├── logo.png
    │   └── [imágenes de productos]
    └── /css/
        └── [estilos compartidos]
```

### 3. Agregar tu primer producto

Copia un archivo de `/productos/` existente:
```bash
cp -r productos/uniclean-oxigeno-activo/ productos/mi-producto/
```

Edita `/productos/mi-producto/index.html`:
- Cambia títulos
- Actualiza descripción
- Reemplaza enlace de Mercado Libre
- Personaliza características

### 4. Subir cambios
```bash
git add .
git commit -m "Agregar nuevo producto: Mi Producto"
git push origin main
```

**Tu sitio se actualizará automáticamente en 5-10 segundos.**

---

## 📦 Productos Incluidos (Ejemplos)

| Producto | Slug | Categoría |
|----------|------|-----------|
| UniClean - Oxígeno Activo | `uniclean-oxigeno-activo` | Aseo Premium |
| Smartwatch Pro | `smartwatch-pro` | Tecnología |
| Almohada Ergonómica | `almohada-ergonomica` | Bienestar |
| Lámpara LED Inteligente | `lampara-led-inteligente` | Hogar |

**Para agregar un nuevo producto:**
1. Crea carpeta: `/productos/nombre-producto/`
2. Copia `index.html` de ejemplo
3. Personaliza contenido
4. Push a GitHub

---

## 🎨 Personalización

### Cambiar Colores Principales
Edita el `<style>` en cualquier `index.html`:
```css
/* Color principal actual */
linear-gradient(135deg, #1e3a8a 0%, #dc2626 100%)

/* Tu gradiente personalizado */
linear-gradient(135deg, #tucolor1 0%, #tucolor2 100%)
```

### Cambiar Logo/Emojis
En el header:
```html
<div class="logo">
    <span class="logo-icon">🛒</span>  <!-- Cambiar este emoji -->
    <span>TuCompraOK</span>
</div>
```

### Agregar Más Categorías
En `index.html`, agrega filtro:
```html
<button class="filter-btn" data-filter="tu-categoria">🎯 Tu Categoría</button>
```

Y asigna productos a ella en el array `productos`:
```javascript
{
    categoria: "tu-categoria",
    // ...resto de datos
}
```

---

## 📊 Métricas y Tracking

### Google Analytics
Agrega a cada página (antes de `</head>`):
```html
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

### Meta Pixel
Para rastrear clics a Mercado Libre:
```html
<img height="1" width="1" style="display:none" 
  src="https://www.facebook.com/tr?id=TU_PIXEL_ID&ev=PageView" />
```

---

## 🔗 Conectar Dominio Propio

### En GitHub
1. Settings → Pages
2. Custom domain: `tucompraok.online`
3. Save

### En tu registrador (Namecheap, GoDaddy, etc.)
Añade estos DNS records:
```
CNAME: www.tucompraok.online → tucompraok.github.io

A Records:
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

**Espera 24-48 horas para propagación.**

---

## 🎯 Estrategia de Marketing

### Campanías Meta Ads
**Presupuesto recomendado:** $100-200/mes

**Segmentación:**
- Audiencia 1: Interesados en hogar limpio
- Audiencia 2: Tech enthusiasts
- Audiencia 3: Bienestar y salud

**Landing URLs:**
- Principal: `https://tucompraok.online/`
- Producto específico: `https://tucompraok.online/productos/uniclean-oxigeno-activo/`

### Métricas a Monitorear
- CTR a Mercado Libre (objetivo: >3%)
- Costo por clic (CPC)
- Conversión en Mercado Libre
- ROAS (Return on Ad Spend)

---

## 📝 Checklist de Implementación

- [ ] Repositorio creado
- [ ] Landing principal funcionando
- [ ] Primer producto agregado
- [ ] GitHub Pages activado
- [ ] Dominio conectado
- [ ] Sitemap.xml creado
- [ ] Google Search Console verificado
- [ ] Meta Pixel instalado
- [ ] Primeras campañas lanzadas
- [ ] Analytics configurado

---

## 🆘 Troubleshooting

**¿Los cambios no aparecen?**
- Limpia caché: `Ctrl+Shift+R` (Windows) o `Cmd+Shift+R` (Mac)
- Espera 10 segundos después de push

**¿El dominio no funciona?**
- Verifica DNS settings
- Espera hasta 48 horas para propagación

**¿Las imágenes no cargan?**
- Usa rutas relativas: `/assets/img/imagen.jpg`
- Asegúrate que el archivo existe

**¿Problemas con Mercado Libre?**
- Verifica que el enlace sea correcto
- Abre en incógnito para evitar caché
- URL debe ser la completa del producto

---

## 📈 Próximos Pasos

1. **Contenido:** Agrega 10-15 productos
2. **SEO:** Optimiza meta tags y descripción
3. **Ads:** Lanza campañas segmentadas
4. **Análisis:** Revisa métricas semanalmente
5. **Escalado:** Aumenta presupuesto si ROAS > 2

---

## 💡 Tips Finales

- Mantén el diseño simple y rápido
- Cada página debe cargar en <2 segundos
- CTA claros: "Comprar en Mercado Libre"
- Mobile-first: 70% tráfico viene de móvil
- Actualiza productos cada semana

---

## 📄 Licencia

Libre para usar, modificar y compartir. No incluye productos específicos, solo estructura.

---

**Creado para emprendedores que valorizan la velocidad y la economía.** 🚀

¿Preguntas? Abre un issue en el repositorio.
