# OmniBiblia — Página oficial «Próximamente»

**Dirección oficial prevista:** https://omnibiblia.dofepro.do/  
**Lema:** Tu Biblia en Todo Lugar.  
**Creador y responsable del proyecto:** Domingo Feliz, República Dominicana.  
**Contacto:** dofeprotech@gmail.com

Este repositorio aloja **exclusivamente la página pública informativa** de OmniBiblia.
No contiene la aplicación principal, bases de datos, credenciales, archivos bíblicos
RVR1960, APK, audios, materiales multimedia de terceros ni secretos.

OmniBiblia es una iniciativa independiente en desarrollo. La aplicación pública
se encuentra temporalmente suspendida durante las revisiones técnicas,
de seguridad y derechos de contenido. No se anuncia una fecha definitiva.

## Identidad y derechos

© 2026 Domingo Feliz. Derechos reservados sobre los elementos originales de esta
página. Consulte `LICENSE` y `aviso-legal.html`.

La denominación OmniBiblia identifica el proyecto, pero **no se presenta como marca
registrada**. El registro de una marca es un procedimiento independiente ante
la autoridad competente. Este sitio y el SEO no sustituyen ese registro.

El código y otros elementos de la aplicación principal requieren una decisión
separada sobre su régimen de licencia. La página pública no concede derechos
sobre traducciones bíblicas, prédicas, audios, videos, imágenes ni otros recursos
de terceros.

## Publicación gratuita con GitHub Pages

1. Crear un repositorio NUEVO y **público** (por ejemplo `OmniBiblia-Proximamente`) bajo la cuenta `Dofepro-Tech`.
2. Subir **solo** los archivos de esta carpeta a la raíz de ese repositorio. No subir
   por accidente la carpeta `.git`, `src`, `public/data`, APK, `.env` ni nada del
   repositorio privado `OmniBiblia`.
3. En GitHub, `Settings → Pages → Build and deployment → Deploy from a branch`
   y seleccionar rama `main`, carpeta `/ (root)`.
4. Primero comprobar el sitio publicado en su URL temporal de GitHub Pages. Verificar
   que no haya ningún texto bíblico protegido ni descargas heredadas.
5. Verificar la propiedad del dominio ante GitHub; añadir en `Settings → Pages → Custom domain`
   el subdominio `omnibiblia.dofepro.do`. No modificar DNS antes de asignar el dominio
   en GitHub. La interfaz puede generar el archivo `CNAME`. El paquete NO incluye ese archivo activo para permitir primero la prueba de la URL temporal. Consulta `CONFIGURAR-DOMINIO.txt`.
6. En el proveedor DNS de `dofepro.do`, crear un registro `CNAME` para el host
   `omnibiblia` apuntando a `dofepro-tech.github.io` (NO al repositorio privado,
   ni a Render ni a una carpeta). No tocar el dominio raíz `dofepro.do`.
7. Comprobar resolución, `HTTPS`, certificado, contenido HTML, canonical y sitemap.
   Habilitar `Enforce HTTPS` al estar disponible.
8. Dar de alta el sitio en Google Search Console utilizando verificación DNS de
   la propiedad que te pertenece. Enviar `https://omnibiblia.dofepro.do/sitemap.xml`
   y solicitar indexación cuando HTTPS y la página funcionen.
9. Preparar aparte la redirección 301/308 desde `bibliadj.dofepro.do` una vez la
   nueva página esté comprobada. No reactivar Render con la aplicación protegida,
   ni redirigir a un servidor que exponga RVR1960.

**Importante:** No manipules el repositorio `Dofepro-Tech/OmniBiblia` (privado)
ni el repositorio `Dofepro-Tech.github.io` (contiene un APK antiguo pendiente de
restringir). Este repositorio nuevo no sustituye la solución del APK antiguo.

## Lista de verificación SEO

- `title`, `meta description`, `lang=es-DO`, meta `author`, canonical coherente.
- Open Graph, Twitter Card, vista previa social `og-image.png`.
- JSON-LD `WebSite` con `creator` y `publisher` atribuibles a Domingo Feliz.
- `robots.txt`, `sitemap.xml`, favicon, página 404, enlaces internos funcionales.
- HTTP 200 y HTTPS válido en las URLs públicas, sin `noindex`.
- Confirmar que Google Search Console refleje la propiedad verificada.
- Revisar que los títulos, descripciones y enlaces coincidan con el contenido real.
- No hacer afirmaciones de «marca registrada» ni colocar el símbolo ®.

## Comprobación local

Puedes abrir `index.html` en un servidor HTTP estático; con Python instalado:

```powershell
python -m http.server 8080
```

Visitar `http://localhost:8080/` desde la carpeta de este repositorio.
El sitio no necesita npm, Vite, Node, claves ni backend.

## Identidad visual

La marca gráfica basada en un libro abierto incluida aquí es **provisional**.
Debe sustituirse por el logotipo oficial de OmniBiblia si se dispone del archivo
original con los derechos y calidad adecuados. Revisar el diseño final antes
de publicar.
