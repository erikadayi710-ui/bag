# 📱💻 Auly Regalos & Bolsos - App Móvil y Página Web

Esta carpeta contiene la aplicación completa configurada para funcionar **tanto en Móviles (Android e iOS) como en la Página Web**.

---

## 🚀 Opciones de Uso:

### 1. Como Página Web (Subir a Cloudflare Pages, Netlify, o Servidor Web):
* La carpeta `www/` contiene `index.html`.
* Puedes subir directamente la carpeta o subir el archivo ZIP a **Cloudflare Pages**, **Vercel** o **GitHub Pages**.
* En el navegador, la aplicación incluye un **selector superior** para cambiar entre el **Marco Móvil (iPhone)** y la **Pantalla Completa Web**.

### 2. Como App Móvil Nativa (Android / iOS con Capacitor):
Para empaquetar esta carpeta como una App nativa para Android (`.apk`) o iOS (`.ipa`):

```bash
# 1. Instalar Capacitor en la carpeta
npm install @capacitor/core @capacitor/cli @capacitor/android @capacitor/ios

# 2. Inicializar y agregar plataformas móviles
npx cap init "Auly Regalos" "com.auly.regalos" --web-dir=www
npx cap add android
npx cap add ios

# 3. Sincronizar archivos
npx cap sync

# 4. Abrir en Android Studio o Xcode para generar el paquete de la App
npx cap open android
npx cap open ios
```
