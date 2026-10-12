# Auditoría pública inicial — 12 de octubre de 2026

Estado: revisión del website documentada; auditoría integral de Instagram/Facebook y cambios externos pendientes de acceso. No se ha publicado ni programado contenido.

## Datos confirmados por el cliente

**ZIP 75051. Lunes a viernes 8:00 AM–5:00 PM. Sábados con cita previa.** En inglés: `Monday–Friday, 8:00 AM–5:00 PM. Saturday by appointment.` No inferir horario del domingo.

North Metal Design LLC. 2125 W Pioneer Pkwy, Suite D2, Grand Prairie, TX 75051. 682-282-7221. shop@northmetaldesign.com. https://northmetaldesign.com/. Instagram: https://www.instagram.com/northmetaldesignllc/. Facebook: https://www.facebook.com/northmetaldesignllc.

## Alcance y evidencia

Se consultaron Home, Portfolio, Contact Us, Safe Closet, About Us y 11 páginas de categorías enlazadas desde imágenes del portfolio. Las respuestas consultadas fueron HTTP 200. Se guardaron HTML, inventarios y textos. Además se comprobaron 26 URLs internas del menú y enlaces relacionados: todas respondieron HTTP 200, incluida /mailbox/. Esto valida acceso al destino, no el contenido de cada página ni el funcionamiento de formularios. No se enviaron formularios ni mensajes de prueba.

Hay cuatro capturas completas útiles del website —home, portfolio, contacto y Safe Closet— y cinco capturas de detalle: contacto, footer con ZIP incorrecto, copy ajeno en Safe Closet, horario de Safe Closet y estadísticas del home. Ver `EVIDENCE/ORIGINALS` y `evidence_register.csv`.

Los recursos se obtuvieron con HTTPS y verificación de certificado mediante urllib y se renderizaron en Chromium. Las imágenes del CDN WordPress propio se cargaron desde sus URLs originales en northmetaldesign.com porque i0.wp.com está bloqueado. No se desactivó TLS. Los fallos de recursos secundarios están registrados en los resultados de captura; estas imágenes no prueban funcionamiento de formularios o integraciones.

## Hallazgos

| Prioridad | Evidencia | Acción preparada | Estado |
| --- | --- | --- | --- |
| Alta | Contact Us muestra 75051; footer y Safe Closet muestran 75017 | Unificar a 75051, confirmado por el cliente | No aplicado |
| Alta | Contact Us/About Us: lunes–viernes 8–5; Safe Closet: lunes–sábado 9:30–6:30 | Unificar e incluir Saturday by appointment | No aplicado |
| Alta | Safe Closet contiene texto sobre Ozlockers, sizing, colours, accessories y power options | Sustituir por descripción específica de Safe Closet | Propuesta preparada |
| Alta | Safe Closet promete maximum security, impossible for intruders y protección durante desastres | Revisar respaldo técnico; no reutilizar garantías absolutas en redes | Pendiente documentación |
| Media | Home afirma 90+ team members, 2K+ proyectos, cientos de premios/certificados y 100% satisfacción | Validar antes de mantener o reutilizar cifras | No se declaran falsas; faltan respaldos |
| Media | Home usa Save Your Budget y fair pricing | Reorientar a custom work, precision y craftsmanship | Propuesta de copy |
| Media | Imagen de Mailbox en Portfolio enlaza a /tables/; título enlaza a /mailbox | /mailbox/ responde HTTP 200; corregir destino de la imagen | No aplicado |
| Media | Las 12 imágenes del portfolio tienen alt vacío en el HTML analizado | Preparar alt descriptivo por imagen verificada | Pendiente |
| Media | Contact Us también muestra estimates@northmetaldesign.com | Confirmar su función antes de sustituir el email principal | shop@ sigue siendo el contacto confirmado |

## Instagram y Facebook — revisión limitada

Instagram: metadatos públicos muestran North Metal Design LLC, @northmetaldesignllc y `Where innovation meets craftsmanship.` En esta consulta también aparecen 365 followers, 205 following y 335 posts. No equivalen a Insights ni a una revisión visual del feed.

Facebook: metadatos públicos muestran `North Metal Design | Grand Prairie TX`, 210 followers y `Crafting excellence in metal. North Metal Design transforms visions into masterpieces.` No constituyen una revisión completa de About, categorías, botones o publicaciones.

Los textos públicos son generales: no explican directamente la oferta, audiencia ni Safe Closet. `CONTENT/profile_proposals.md` prepara una mejora de posicionamiento sin cambiar cuentas.

El HTML público es accesible, pero Instagram produjo una vista vacía por recursos bloqueados y Facebook no completó la navegación visual. La captura vacía de Instagram no se cuenta como evidencia útil. Recursos adicionales necesarios: static.cdninstagram.com, static.xx.fbcdn.net, scontent-msp1-1.cdninstagram.com y scontent-msp1-1.xx.fbcdn.net. Se guardaron en el borrador; su acceso todavía no está validado tras aplicar cambios.

No hay sesión autorizada de Meta Business Suite ni herramientas conectadas para administrar Meta, Google Drive, Google Business o WordPress. No se revisaron mensajes, Insights, Archive ni configuraciones privadas.

## Assets y contenido

Se descargaron **88 archivos** del sitio oficial: 12 imágenes de portada de categorías y 76 archivos de galerías. Hay **79 contenidos binarios distintos por SHA-256**; los duplicados se mantienen trazables. Los archivos conservan sus bytes originales. Se excluyeron logos y no se descargaron imágenes de otros dominios como material de publicación.

Inventarios: `RESEARCH/portfolio_asset_inventory.json` y `RESEARCH/gallery_original_inventory.json`. Las categorías no confirman ubicación, cliente, material, alcance exacto de fabricación ni que todas las versiones del sitio sean fotografías sin edición. Los captions no infieren estos datos.

Se inspeccionaron imágenes para preparar diez captions en inglés y diez conceptos de Stories en `CONTENT/first_10_drafts.md`. Son borradores editoriales: no están programados y no hay derivados finales 1080 × 1080, Stories gráficos ni tríptico terminado. Los logos actuales de NEW siguen pendientes de acceso.

## Siguiente ejecución

1. Aplicar los dominios de recursos Meta en environment settings y reintentar las vistas públicas.
2. Habilitar acceso autorizado a Meta Business Suite y al administrador del website para aplicar las correcciones confirmadas. Login/MFA requieren intervención del usuario; nunca pedir credenciales en chat.
3. Facilitar logos actuales de North Metal Design de NEW y el archivo original del logo de MGT Systems para el reporte. G:\My Drive no está montado; la estructura de assets es local.
4. Terminar revisión visual de publicaciones antes de archivar. No eliminar.
5. Preparar derivados y tríptico, mostrar preview y validar orden; obtener aprobación específica del tríptico antes de publicarlo.

## Estado del trabajo

Reporte con marca MGT Systems y mención de colaboración con **Apsolife Media Studios LLC** en social media. Logo visible en chat, pendiente de archivo accesible para exportar el reporte final. Preguntas y solicitudes al cliente en español.

Cambios externos: 0. Publicaciones programadas: 0. Publicaciones publicadas: 0. Posts archivados: 0. La preparación local y su evidencia se registran por separado de implementaciones.
