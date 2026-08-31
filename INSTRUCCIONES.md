# Instrucciones de uso y mantenimiento

Este repositorio es una dependencia operativa de una encuesta implementada en Qualtrics. Su función es alojar imágenes de estímulos y otros archivos estáticos que pueden estar referenciados directamente desde la encuesta.

No es el repositorio principal de investigación: el diseño experimental, los datos de investigación, el análisis empírico y los materiales de reproducibilidad se mantienen en el repositorio específico del experimento de elección de rotaciones agrícolas.

## Regla principal

Mientras la encuesta esté activa o pueda volver a utilizarse, **no cambies rutas existentes sin comprobar primero todas las referencias en Qualtrics**.

En particular:

- no renombres archivos de estímulos existentes;
- no muevas esos archivos a otras carpetas;
- no elimines archivos que todavía puedan estar referenciados por Qualtrics;
- no cambies el nombre del repositorio ni la rama predeterminada sin actualizar y probar todas las referencias;
- si cambia de forma sustantiva el contenido visual de un estímulo, preferí agregar un archivo nuevo con un nombre nuevo y estable antes que reemplazar silenciosamente el existente.

## Procedimiento seguro para actualizar un estímulo

1. Identificá todas las preguntas de Qualtrics y reglas de datos incrustados que utilicen el archivo actual.
2. Agregá el nuevo estímulo con un nombre de archivo nuevo y estable, siempre que sea posible.
3. Actualizá en Qualtrics la referencia correspondiente.
4. Previsualizá y probá la encuesta de principio a fin.
5. Eliminá un estímulo antiguo únicamente después de confirmar que ya no está referenciado en ninguna versión activa o reutilizable de la encuesta.

## Qué debe permanecer fuera de este repositorio

No uses este repositorio como ubicación canónica para:

- datos a nivel de participante;
- código principal de procesamiento de datos;
- código vigente de diseño experimental;
- análisis empírico;
- paquete de replicación para publicación.

Esos componentes pertenecen al repositorio de investigación correspondiente.

## Cierre de la encuesta

Cuando la encuesta quede cerrada de forma permanente y no vaya a reutilizarse, este repositorio puede pasar a ser un archivo histórico. Antes de archivarlo, preservá un registro de la versión final de Qualtrics y de los archivos de estímulos exactos utilizados en esa versión.

## Criterio de mantenimiento

El objetivo principal es preservar la estabilidad de las URL y la trazabilidad de los estímulos utilizados. Ante cualquier duda, es preferible conservar un archivo antiguo y agregar uno nuevo antes que modificar o eliminar una dependencia que pueda romper la encuesta.
