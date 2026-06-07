# AkuaSea — Landing Page

Sitio web oficial de AkuaSea, proveedor de calzado acuático para hotelería.

## Estructura del proyecto

```
akuasea/
├── index.html        ← Página principal
├── images/
│   ├── logo.jpeg
│   ├── tenis-negro.png
│   ├── zapato-rosa.png
│   ├── sandalia-merida.png
│   └── sandalia-bali.png   (agregar más fotos aquí)
└── README.md
```

## Cómo agregar más fotos de productos

1. Coloca las imágenes en la carpeta `images/`
2. En `index.html`, busca el comentario `<!-- PRODUCTS DETAIL -->` o la sección de categorías
3. Actualiza el `src` de los `<img>` con el nombre del nuevo archivo

---

## Despliegue en GitHub + Netlify

### Paso 1 — Subir a GitHub

1. Ve a [github.com](https://github.com) y crea una cuenta (si no tienes)
2. Haz clic en **"New repository"** (botón verde)
3. Nombra el repo: `akuasea-web`
4. Déjalo **Public**, sin README adicional
5. Crea el repositorio

### Paso 2 — Subir los archivos

**Opción A — Desde la web de GitHub (sin código):**
1. Dentro del repo, haz clic en **"uploading an existing file"**
2. Arrastra toda la carpeta `akuasea/` (o los archivos sueltos)
3. Haz clic en **"Commit changes"**

> ⚠️ Asegúrate de que las imágenes queden en una carpeta `images/` dentro del repo.

**Opción B — Con Git (terminal):**
```bash
cd akuasea/
git init
git add .
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/akuasea-web.git
git push -u origin main
```

### Paso 3 — Conectar con Netlify

1. Ve a [netlify.com](https://netlify.com) y crea una cuenta (gratis, puedes usar tu cuenta de GitHub)
2. Haz clic en **"Add new site" → "Import an existing project"**
3. Elige **GitHub** y autoriza el acceso
4. Selecciona el repo `akuasea-web`
5. En configuración de build, deja todo vacío (es HTML estático):
   - Build command: *(dejar en blanco)*
   - Publish directory: `.` o dejar vacío
6. Haz clic en **"Deploy site"**

Netlify te dará una URL tipo `https://akuasea-web.netlify.app` en segundos ✅

### Paso 4 — Conectar tu dominio propio

1. En Netlify, ve a **Site settings → Domain management**
2. Haz clic en **"Add a domain"**
3. Escribe tu dominio (ej. `akuasea.com.mx`)
4. Netlify te mostrará los nameservers o registros DNS a configurar
5. Entra al panel de tu proveedor de dominio y actualiza esos registros
6. En 24-48 hrs estará activo con SSL gratuito ✅

---

## Notas técnicas

- El sitio es 100% HTML/CSS/JS estático — no requiere servidor ni backend
- SSL (HTTPS) se configura automáticamente en Netlify
- El formulario de contacto abre WhatsApp con los datos prellenados
- Los botones flotantes conectan directamente a WhatsApp y llamada

---

## Personalización pendiente

Cuando tengas más fotos de productos:
- Agrega las imágenes a `images/`
- Actualiza las tarjetas de categorías con las imágenes correctas por modelo

Contacto técnico: Ricardo Aceves (desarrollador)
