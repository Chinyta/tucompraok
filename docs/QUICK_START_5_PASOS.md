# ⚡ QUICK START: 5 Pasos para IR LIVE HOY

**Tiempo estimado: 15-20 minutos**

---

## 🎯 Paso 1: Crear Repositorio en GitHub (3 minutos)

### A. Crear la cuenta (si no tienes)
1. Ve a https://github.com/signup
2. Crea tu cuenta gratis
3. Verifica email

### B. Crear el repositorio
1. Ve a https://github.com/new
2. **Nombre:** `tucompraok.github.io` (exactamente así, no cambiar)
3. Marca como **Public**
4. **NO** inicialices con README (lo haremos nosotros)
5. Click **"Create repository"**

### ✅ Listo: Ya tienes tu repositorio creado

---

## 📁 Paso 2: Subir tu Landing Principal (4 minutos)

### Opción A: Interfaz Web (Más Fácil)

1. En tu repositorio, click en **"Add file"** → **"Upload files"**
2. Descarga el archivo: `tucompraok-index.html` (de los archivos que te presenté)
3. **Renombra el archivo a:** `index.html`
4. Arrastra el archivo al navegador o click en **"Choose your files"**
5. Baja al final y click **"Commit changes"**

### Opción B: Con Git (Más Rápido si ya tienes)

```bash
# En tu computadora
git clone https://github.com/tu-usuario/tucompraok.github.io.git
cd tucompraok.github.io

# Copia tu archivo descargado como:
# tucompraok-index.html → index.html

# Sube a GitHub
git add index.html
git commit -m "Add landing principal"
git push origin main
```

### ✅ Listo: Tu landing principal está online en:
**https://tucompraok.github.io**

---

## 🛍️ Paso 3: Agregar tu Primer Producto (5 minutos)

### A. Crear Carpeta de Producto
En GitHub:
1. Click **"Add file"** → **"Create new file"**
2. En el campo de nombre escribe: `productos/uniclean-oxigeno-activo/index.html`
   - Esto crea automáticamente las carpetas
3. Haz click en la parte de contenido del editor

### B. Copiar Contenido del Template
1. Descarga: `tucompraok-producto-template.html`
2. Abre con un editor de texto (VS Code, Notepad++, etc.)
3. Copia **todo el contenido**
4. En GitHub, pega el contenido en el editor
5. Click **"Commit new file"**

### ✅ Listo: Tu primer producto está en:
**https://tucompraok.github.io/productos/uniclean-oxigeno-activo/**

---

## 🔗 Paso 4: Conectar Enlaces de Mercado Libre (2 minutos)

### En cada landing de producto:

1. Abre el archivo `index.html` del producto (edit button)
2. Busca: `href="https://mercadolibre.com.ar/..."`
3. Reemplaza con tu enlace real de Mercado Libre:
   ```html
   <!-- BUSCA ESTO: -->
   <a href="https://mercadolibre.com.ar/..." target="_blank" class="btn btn-primary">

   <!-- REEMPLAZA CON: -->
   <a href="https://mercadolibre.com.ar/mip/tuproducto123456" target="_blank" class="btn btn-primary">
   ```

4. **Cómo obtener el enlace:**
   - Ve a tu producto en Mercado Libre
   - Copia la URL de la barra de dirección
   - Pégala en el HTML

### ✅ Listo: Los botones ya van a Mercado Libre

---

## 🌐 Paso 5: (OPCIONAL) Conectar tu Dominio tucompraok.online (3 minutos)

### A. En GitHub
1. Abre Settings del repositorio
2. Busca **"Pages"** en el menú izquierdo
3. Bajo "Build and deployment":
   - Branch: `main` / root
4. Baja a **"Custom domain"**
5. Escribe: `tucompraok.online`
6. Click **"Save"**

### B. En tu Registrador de Dominio (Namecheap, GoDaddy, etc.)
1. Abre la sección **DNS** o **Name Servers**
2. Busca **CNAME** o **A Records**
3. Agrégalos así:
   ```
   CNAME: www.tucompraok.online → tucompraok.github.io
   
   A Records (agregar 4):
   185.199.108.153
   185.199.109.153
   185.199.110.153
   185.199.111.153
   ```
4. Guarda

### ⏱️ Espera 24-48 horas
Luego tu sitio estará en: **https://tucompraok.online**

---

## ✅ CHECKLIST: ¿Está TODO LISTO?

- [ ] Repositorio `tucompraok.github.io` creado
- [ ] `index.html` subido (landing principal funciona)
- [ ] Primera carpeta de producto creada (`/productos/uniclean...`)
- [ ] Template de producto pegado en la carpeta
- [ ] Enlaces de Mercado Libre actualizados
- [ ] (Opcional) Dominio conectado

---

## 🚀 ¡YA ESTÁS ONLINE!

Tu tienda está en:
- **https://tucompraok.github.io** ← ACCESO INMEDIATO
- **https://tucompraok.online** ← Si conectaste dominio

---

## 📈 Próximos Pasos (Después de hoy)

### Mañana: Agregar 3-5 Productos más
1. Copia la carpeta `/productos/uniclean.../` 
2. Renómbrala con tu nuevo producto
3. Edita el `index.html` con tus datos
4. Push a GitHub

### Esta Semana: Configurar Ads
1. Crear campañas en Meta Ads
   - Presupuesto: $20-50 (test)
   - Audiencia: Tu mercado objetivo
   - URL: Tu landing principal o de producto
2. Añadir pixel de seguimiento

### Este Mes: Optimizar
1. Ver qué productos se convierten mejor
2. Mejorar descripción de los que venden menos
3. Aumentar presupuesto de ads si ROAS > 1.5

---

## 🆘 Si Algo Falla

| Problema | Solución |
|----------|----------|
| "El archivo no se sube" | Intenta navegador diferente o recarga la página |
| "index.html no aparece en raíz" | Verifica que el nombre sea exactamente `index.html` |
| "Cambios no se ven" | Recarga con `Ctrl+Shift+R` (Windows) o `Cmd+Shift+R` (Mac) |
| "Enlace de Mercado Libre muerto" | Verifica que el URL sea correcto y empiece con `https://` |
| "Dominio no funciona" | Espera 48h, verifica DNS records coincidan exactamente |

---

## 💡 Tips de Oro

✨ **Hazlo Simple:**
- No necesitas perfección en diseño, necesitas conversión
- Cada página debe cargar en <2 segundos
- Botones grandes y claros: "COMPRAR EN MERCADO LIBRE"

✨ **Actualiza Cada Semana:**
- Agrega 1 nuevo producto
- Mejora descripción de un antiguo
- Revisa métricas de Mercado Libre

✨ **Invierte en Ads Inteligentemente:**
- Comienza con $20-30/semana
- Segmenta por categoría
- Mantén ROAS > 1.5 (mínimo)

---

## 📞 Recursos

- **GitHub Pages Docs:** https://pages.github.com/
- **Mercado Libre:** https://mercadolibre.com.ar
- **Meta Ads:** https://www.facebook.com/ads/

---

**¿Listo? Comienza con el Paso 1 en los próximos 5 minutos. 
Tu tienda online estará LIVE en menos de 20 minutos.** 🚀

*Hecho para emprendedores que valorizan la velocidad.*
