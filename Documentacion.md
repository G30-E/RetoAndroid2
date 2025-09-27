# retoandroid





PROMPT: Especificación completa para la app “¿Qué Comer Hoy?” CONTEXTO Y OBJETIVO Contexto: Aplicación Android sencilla donde el usuario toca un botón para recibir una recomendación de receta aleatoria desde la API pública TheMealDB. La app muestra imagen, nombre, categoría, área de origen, lista de ingredientes con medidas, instrucciones, y enlaces (YouTube/Source). Debe permitir personalizar sugerencias con filtros (p. ej., tipo de dieta, tiempo disponible, ingredientes en casa) y un modo “mood” usando prompts para ajustar la recomendación. Objetivo: Obtener recetas al azar (y/o filtradas) desde TheMealDB. Renderizar imagen de la receta (thumb) con Glide. Ofrecer acciones: “Otra receta”, “Guardar en favoritos” REQUISITOS FUNCIONALES Entradas: Botón “¿Qué comer hoy?” para pedir receta aleatoria. Procesos: Llamar a TheMealDB: Aleatoria: /api/json/v1/1/random.php Por id: /lookup.php?i={id} Parsear JSON y construir modelo de dominio (Meal + lista de ingredientes/medidas). Cargar imagen strMealThumb con Glide (caché por defecto). Aplicar reglas de personalización a partir del prompt del usuario (“tengo 20 minutos y antojo de algo picante y barato”) → traducir a filtros (p. ej., evitar recetas con > X pasos) Gestionar estado: Loading / Success / Empty / Error. Persistir “Favoritos” en base local (Room) y exponer listado. Salidas: Pantalla con tarjeta de receta: imagen, título, categoría, área, ingredientes+medidas, instrucciones Snackbar/Toast para estados (guardado en favoritos, error de red, etc.). Vista de Favoritos (opcional): lista con miniatura e ingreso al detalle.

APIs/Librerías: API de TheMealDB

Permisos: android.permission.INTERNET (único requerido).

Barra de progreso mientras carga. Guardar/recuperar último resultado (restauración tras rotación opcional). Persistencia:

Acciones: agregar/quitar favorito





 

resultado obtenido: este me dio el programa completo







problemas encontrados: al hacer la primer prueba el programa me dio problemas de red pero fue por que no había establecido los permisos de internet En AndroidManifest.xml






reflexión final: la ia es algo muy sorprendente ya que con darle instrucciones claras puede hacer cosas que a nosotros nos llevarían horas

