# CRM Escuela Ministerial Fuente de Vida

Sistema de gestión escolar (cursos, alumnos, asistencia, pagos, calificaciones,
constancias, reportes, comunicación y conexiones con Google). App web de un solo
archivo (`index.html`). Funciona en modo local (navegador) o en modo nube
(Firebase, multi-escuela con login por usuario).

## Cómo correrlo
- **Local rápido:** abre `index.html` con doble clic (las conexiones a Google/nube NO funcionan así).
- **Con conexiones (localhost):** en esta carpeta, `python3 -m http.server 8000` y abre `http://localhost:8000/`.
- **Publicado (recomendado):** GitHub Pages / Netlify / Firebase Hosting → te da una URL https.

## Notas
- Los datos de los alumnos NO viven en este archivo: en modo local quedan en el navegador,
  y en modo nube en Firestore. Por eso el repo puede ser público sin exponer datos.
- La configuración web de Firebase y la apiKey de Google son públicas por diseño;
  la seguridad la dan las reglas de Firestore y el inicio de sesión.

## Guías de configuración
Dentro de la app, pestaña **Conexiones**: pasos para Google (Calendar/Gmail/Contactos)
y para el modo nube con Firebase (incluye las reglas de seguridad).
