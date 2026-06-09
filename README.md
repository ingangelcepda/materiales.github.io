# Representación Gráfica y Tecnología de los Materiales

Breve guía del contenido y cómo probarlo en un entorno local (WAMP).

## Contenido
- `Index.html` — Página de inicio (versión principal).  
- `IndexII.html` — Plataforma interactiva del curso: semanas, competencias, videos y ejercicios.  

## Cómo abrir el proyecto
1. Asegúrate de tener WAMP (o cualquier servidor local) instalado y ejecutándose.  
2. Coloca esta carpeta dentro de la raíz `www` de WAMP (ya debería estar en `C:\wamp64\www\UNACOM`).  
3. Abre en tu navegador la ruta local (ajusta espacios codificados si es necesario):  

```
http://localhost/UNACOM/Representación%20Gráfica%20y%20Tecnología%20de%20los%20Materiales/IndexII.html
```

## Ver y probar los videos
- La galería usa enlaces de YouTube; las miniaturas se generan automáticamente desde el ID (`https://img.youtube.com/vi/<ID>/hqdefault.jpg`).  
- Para reproducir un video, abre la pestaña de `Competencia`, selecciona un video y haz clic en "Ver aquí" (se abre en el reproductor embebido).  
- Si la miniatura no carga, se usa un fallback genérico dentro de la página.

## Editar contenido multimedia y ejercicios
- El contenido principal está definido en el objeto `compMetadata` dentro de `IndexII.html`. Allí puedes:  
  - Actualizar `videos` (cada entrada debe tener `title`, `desc`, `url`, `thumb`).  
  - Editar `theory` y `exercises` (cada ejercicio puede incluir `solution` en HTML).  

Ejemplo de entrada de video:

```
{ title: "Título", desc: "Descripción", url: "https://www.youtube.com/watch?v=ID", thumb: "ID" }
```

## Solicitudes y notas del autor
- Las soluciones de ejercicios (`ex.solution`) se muestran mediante un control `toggle` o `<details>` según la preferencia.  
- Cambios visuales y listas de videos se editan directamente en `IndexII.html`.  

Si quieres, puedo:
- abrir el archivo y mostrar dónde editar `compMetadata`,  
- o generar una copia mínima del proyecto para pruebas estáticas.

---
Archivo generado automáticamente por el asistente.
