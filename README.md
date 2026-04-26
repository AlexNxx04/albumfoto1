# 💕 Nuestro Álbum — Guía de configuración

Álbum de fotos polaroid compartido en tiempo real para dos personas.

---

## ¿Qué necesitas?

- Una cuenta gratuita en [Firebase](https://firebase.google.com) (de Google)
- Una cuenta en [GitHub](https://github.com) (para publicarlo)

---

## PASO 1 — Crear tu proyecto Firebase (gratis)

1. Ve a **https://console.firebase.google.com**
2. Click en **"Agregar proyecto"**
3. Ponle un nombre (ej: `nuestro-album-amor`)
4. Desactiva Google Analytics si quieres → **Crear proyecto**

### Activar Realtime Database:
5. En el menú izquierdo → **"Realtime Database"**
6. Click **"Crear base de datos"**
7. Elige una región (ej: `us-central1`)
8. Selecciona **"Iniciar en modo de prueba"** → Habilitar

### Copiar tus credenciales:
9. Click en el ⚙️ (Configuración del proyecto) arriba a la izquierda
10. Baja hasta **"Tus apps"** → Click en `</>` (web app)
11. Ponle un nombre → **Registrar app**
12. Copia el bloque `firebaseConfig` que aparece, se ve así:

```js
const firebaseConfig = {
  apiKey: "AIzaSy...",
  authDomain: "tu-album.firebaseapp.com",
  databaseURL: "https://tu-album-default-rtdb.firebaseio.com",
  projectId: "tu-album",
  storageBucket: "tu-album.appspot.com",
  messagingSenderId: "12345678",
  appId: "1:12345678:web:abcdef"
};
```

---

## PASO 2 — Poner tus credenciales en el archivo

1. Abre `index.html` con cualquier editor de texto (Notepad, VS Code, etc.)
2. Busca la línea que dice `const FIREBASE_CONFIG = {`
3. Reemplaza el bloque completo con **tus datos reales de Firebase**

---

## PASO 3 — Subir a GitHub Pages

1. Ve a **https://github.com** e inicia sesión
2. Click en **"New repository"** (repositorio nuevo)
3. Ponle un nombre (ej: `nuestro-album`)
4. Que sea **Public** → **Create repository**
5. Click en **"uploading an existing file"**
6. Sube el archivo `index.html`
7. Click en **"Commit changes"**

### Activar GitHub Pages:
8. Ve a **Settings** (en tu repositorio)
9. Menú izquierdo → **Pages**
10. En "Branch" selecciona **main** → carpeta **/ (root)**
11. Click **Save**
12. Espera 1-2 minutos y tendrás una URL como:
    **`https://tuusuario.github.io/nuestro-album`**

---

## PASO 4 — Compartir con tu novia 💌

1. Manda esa URL a tu novia
2. Ambos entran con el mismo **código de álbum** (inventate uno)
3. ¡Todo lo que uno hace, el otro lo ve en tiempo real!

---

## ¿Cómo funciona?

| Quién | Puede hacer |
|-------|------------|
| 🧑 El novio | Subir fotos (múltiples por página), agregar páginas |
| 🌸 La novia | Escribir cómo se sintió en cada recuerdo |
| Ambos | Ver todo en tiempo real, navegar entre páginas |

---

## Funciones del álbum

- 📸 **Múltiples fotos por página** — sube todas las que quieras
- 🎞️ **Efecto polaroid sepia** — con animación de "revelado"
- 🌸 **Flores decorativas** — al lado de cada página
- 📖 **Páginas como libro** — con efecto de cambio
- 💌 **Escritura en tiempo real** — la novia escribe y el novio ve al instante
- ➕ **Agregar páginas** — sin límite
- 🔄 **Sincronización automática** — sin recargar la página

---

## ¿Problemas?

- **"Error conectando con Firebase"**: Verifica que copiaste bien las credenciales
- **Las fotos no se guardan**: Asegúrate que la base de datos esté en "modo test"
- **Mi novia no ve los cambios**: Revisen que usen exactamente el mismo código de álbum

---

*Hecho con amor 💕*
