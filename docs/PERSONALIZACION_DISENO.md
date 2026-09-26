# 🎨 Guía de Personalización: Colores, Fuentes y Diseño

Este documento te muestra exactamente DÓNDE y CÓMO cambiar los colores, fuentes y elementos visuales de tu tienda.

---

## 🎯 Colores Principales (Los Más Importantes)

### Dónde están
En cada archivo `index.html`, busca la sección `<style>`:
```html
<style>
    /* Aquí están todos los colores */
</style>
```

### Cambiar el Gradiente Principal (Header + Hero)

**BÚSQUEDA:** `linear-gradient(135deg, #1e3a8a 0%, #dc2626 100%)`

Este gradiente aparece en:
1. Header
2. Hero section
3. Botones principales

**Ejemplos de Gradientes Personalizados:**

```css
/* Azul a Verde (Moderno) */
linear-gradient(135deg, #1e40af 0%, #10b981 100%)

/* Naranja a Rojo (Energético - Tu logo) */
linear-gradient(135deg, #f97316 0%, #ef4444 100%)

/* Púrpura a Rosado (Premium) */
linear-gradient(135deg, #7c3aed 0%, #ec4899 100%)

/* Teal a Azul (Tech) */
linear-gradient(135deg, #14b8a6 0%, #0ea5e9 100%)

/* Amarillo a Naranja (Cálido) */
linear-gradient(135deg, #eab308 0%, #f97316 100%)
```

**Cómo cambiar:**
1. Encuentra la línea con el gradiente actual
2. Reemplaza con tu gradiente preferido
3. Guarda el archivo

---

## 🔴 Colores Secundarios

| Elemento | Color Actual | Código | Dónde Cambiarlo |
|----------|-------------|--------|-----------------|
| Botones Rojo | Rojo Brillante | `#dc2626` | Busca `"#dc2626"` |
| Texto Oscuro | Gris Oscuro | `#1f2937` | Busca `"#1f2937"` |
| Fondo | Gris Claro | `#f8f9fa` | Busca `"#f8f9fa"` |
| Bordes | Gris Medio | `#e5e7eb` | Busca `"#e5e7eb"` |
| Badges | Amarillo | `#fef3c7` | Busca `"#fef3c7"` |

### Cambiar Todos los Rojos a tu Color
Usa "Buscar y Reemplazar":
1. Abre el archivo HTML en editor de texto
2. Presiona `Ctrl+H` (Windows) o `Cmd+H` (Mac)
3. Busca: `#dc2626`
4. Reemplaza por tu color (ej: `#f97316` para naranja)
5. Click "Replace All"

---

## 🔤 Fuentes (Tipografía)

### Fuente Actual
El diseño usa **Segoe UI** (sistema operativo):
```css
font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
```

### Cambiar a Google Fonts (Mejor)

**Opción 1: Montserrat (Moderno, Profesional)**

Busca `</head>` en el HTML y agrega ANTES:
```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700&display=swap" rel="stylesheet">
```

Luego cambia el `font-family`:
```css
/* ANTES */
font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;

/* DESPUÉS */
font-family: 'Montserrat', sans-serif;
```

**Opción 2: Inter (Limpia y Rápida)**
```html
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
```
```css
font-family: 'Inter', sans-serif;
```

**Opción 3: Poppins (Amigable)**
```html
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap" rel="stylesheet">
```
```css
font-family: 'Poppins', sans-serif;
```

---

## 📐 Tamaños de Fuentes

| Elemento | Tamaño Actual | Dónde | Código |
|----------|---------------|-------|--------|
| Títulos Grandes (h1) | 42px | Hero section | `font-size: 42px;` |
| Títulos Producto | 32px | Landing producto | `font-size: 32px;` |
| Nombres (h3) | 18px | Cards de producto | `font-size: 18px;` |
| Texto Normal | 16px | Párrafos | `font-size: 16px;` |
| Etiquetas | 14px | Tags | `font-size: 14px;` |

### Hacerlo Más Grande (Menos Profesional pero Más Legible)
Multiplica todos por 1.15:
- 42px → 48px
- 32px → 37px
- 18px → 21px
- 16px → 18px
- 14px → 16px

### Hacerlo Más Pequeño (Más Elegante)
Multiplica todos por 0.85:
- 42px → 36px
- 32px → 27px
- 18px → 15px
- 16px → 14px

---

## 🎨 Cambiar Logo/Emojis

### Logo en Header
Busca:
```html
<div class="logo">
    <span class="logo-icon">🛒</span>  <!-- ESTE EMOJI -->
    <span>TuCompraOK</span>
</div>
```

Cambia `🛒` por:
- `🏪` - Tienda
- `🏬` - Centro comercial
- `🎁` - Regalo
- `💼` - Negocios
- `⭐` - Estrella

### Emojis en Producto
En landing de producto, busca:
```html
<div class="product-image">🧪</div>  <!-- ESTE -->
```

Opciones según categoría:
- **Tecnología:** `💻` `⌚` `📱` `🖥️`
- **Hogar:** `🏠` `🛋️` `💡` `🪴`
- **Bienestar:** `💆` `🧘` `🌿` `💪`
- **Aseo:** `🧴` `🧼` `🧹` `✨`
- **Herramientas:** `🔧` `🔨` `⚙️` `🛠️`

---

## 🔘 Botones: Cambiar Estilos

### Botón Primario (Comprar)
Búsqueda:
```css
.btn-primary {
    background: linear-gradient(135deg, #dc2626 0%, #b91c1c 100%);
    color: white;
}
```

Opciones:
```css
/* Verde (Conversión) */
background: linear-gradient(135deg, #10b981 0%, #059669 100%);

/* Azul (Profesional) */
background: linear-gradient(135deg, #3b82f6 0%, #1e40af 100%);

/* Naranja (Energético) */
background: linear-gradient(135deg, #f97316 0%, #ea580c 100%);
```

### Botón Secundario (Ver Detalle)
```css
.btn-secondary {
    background: white;
    color: #1e3a8a;
    border: 2px solid #1e3a8a;
}
```

Cambiar color del borde:
```css
border: 2px solid #10b981;  /* Verde */
color: #10b981;
```

---

## 💬 Textos para Cambiar Rápido

### Hero Section (Landing Principal)
Busca:
```html
<h1>Productos Premium a Mejores Precios</h1>
<p>Descubre nuestra selección...</p>
```

Reemplaza con:
```html
<h1>Tu nuevo titular aquí</h1>
<p>Tu descripción aquí...</p>
```

### Categorías de Filtros
Busca:
```html
<button class="filter-btn" data-filter="tecnologia">🖥️ Tecnología</button>
<button class="filter-btn" data-filter="bienestar">💆 Bienestar</button>
```

Agrega o cambia categorías:
```html
<button class="filter-btn" data-filter="mi-categoria">🎯 Mi Categoría</button>
```

---

## 🌙 Modo Oscuro

El diseño actual funciona bien en ambos modos. Si quieres optimizar para modo oscuro:

**Agregar al final de `<style>`:**
```css
@media (prefers-color-scheme: dark) {
    body {
        background: #1a1a1a;
        color: #e5e7eb;
    }
    
    .product-card {
        background: #2d2d2d;
    }
    
    footer {
        background: #0f0f0f;
    }
}
```

---

## 📱 Responsive: Cambiar Puntos de Quiebre

En la sección `@media (max-width: 768px)`:
```css
/* Tablets y móviles menores a 768px */
```

Puedes agregar más puntos:
```css
/* Móviles (menos de 480px) */
@media (max-width: 480px) {
    .product-title {
        font-size: 18px;  /* Más pequeño en móvil */
    }
}

/* Tablets grandes (más de 1024px) */
@media (min-width: 1024px) {
    .products-grid {
        grid-template-columns: repeat(4, 1fr);  /* 4 columnas */
    }
}
```

---

## 🎯 Ejemplos de Temas Completos

### TEMA 1: Profesional Azul (Para B2B)
```
Gradiente: #0f172a → #1e3a8a
Botón: #3b82f6
Fuente: Inter
Tamaño: -10% (más compacto)
```

### TEMA 2: Cálido Naranja (Para Hogar)
```
Gradiente: #ea580c → #f97316
Botón: #ea580c
Fuente: Poppins
Tamaño: +10% (más legible)
```

### TEMA 3: Fresco Verde (Para Bienestar)
```
Gradiente: #059669 → #10b981
Botón: #10b981
Fuente: Montserrat
Tamaño: Normal
```

### TEMA 4: Premium Negro (Para Lujo)
```
Gradiente: #1f2937 → #374151
Botón: #f59e0b (Dorado)
Fuente: Inter
Tamaño: Igual
```

---

## ✅ Checklist de Personalización

- [ ] Cambié colores principales al gradiente de mi marca
- [ ] Actualicé la fuente a una más moderna (Google Fonts)
- [ ] Cambié el emoji del logo por algo relevante
- [ ] Actualicé textos del hero (título + descripción)
- [ ] Personalicé los títulos del botón principal
- [ ] Ajusté tamaños si es necesario
- [ ] Revisé en móvil que se vea bien

---

## 💡 Tips Finales

✨ **Menos es Más:**
- No cambies todo a la vez
- Prueba un cambio, espera 10 seg, recarga
- Si algo se ve mal, deshaz (`Ctrl+Z`)

✨ **Usa Contrastes:**
- El texto DEBE contrastar con el fondo
- Botones oscuros con texto blanco
- Botones claros con texto oscuro

✨ **Sé Consistente:**
- Usa máximo 2-3 colores principales
- Mantén la misma fuente en todo
- Los estilos deben ser coherentes

---

**Guarda tu archivo después de cada cambio. 
Presiona `Ctrl+Shift+R` para limpiar caché y ver cambios.** ✨
