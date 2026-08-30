# Manual técnico de uso — Estantería

> ¿Busca instrucciones sencillas para el día a día? Consulte primero la [Guía fácil de Estantería](GUIA_FACIL.md).

Estantería es una aplicación web para organizar libros, controlar sus copias físicas y saber rápidamente si un título está disponible. Funciona en el navegador y no requiere crear una cuenta.

## 1. Abrir la aplicación

Abra el archivo [index.html](index.html) con un navegador moderno, como Microsoft Edge, Google Chrome o Firefox. En la primera apertura verá tres libros de ejemplo; puede conservarlos para aprender o eliminarlos desde cada ficha.

> Importante: el catálogo se guarda en el navegador y dispositivo que esté usando. Antes de cambiar de ordenador o borrar los datos del navegador, descargue una copia de seguridad.

## 2. Conocer la pantalla principal

El menú lateral reúne las secciones principales:

| Sección | Para qué sirve |
| --- | --- |
| **Inicio** | Resume el número de títulos, copias y préstamos activos. También incluye accesos rápidos. |
| **Catálogo** | Muestra todos los libros, permite buscarlos y abrir sus fichas. |
| **Colecciones** | Agrupa libros por sala, tema, club de lectura, edad o cualquier criterio útil. |
| **Préstamos** | Registra quién tiene cada ejemplar y permite devolverlo. |
| **Inventario** | Lista cada copia física, con su código, ubicación y estado. |
| **Datos y ajustes** | Cambia el nombre de la biblioteca, importa, exporta o borra los datos. |

La barra de búsqueda superior permite localizar un libro por título, autor, ISBN o etiqueta. También puede pulsar `Ctrl + K` para colocar el cursor directamente en ella.

## 3. Añadir un libro

Pulse **Añadir libro** en la parte superior o **Alta manual** en Inicio. Se abrirá una ficha.

### Añadir mediante ISBN

1. Escriba el ISBN en el campo superior. Puede incluir guiones o espacios.
2. Pulse **Completar por ISBN**.
3. Si se encuentra información, se rellenarán título, autor, año y editorial automáticamente.
4. Revise la información y complete la colección, ubicación, etiquetas, notas y número de copias.
5. Pulse **Guardar libro**.

Para utilizar la consulta automática se necesita conexión a internet. Si no se encuentra el ISBN o no hay conexión, rellene la ficha manualmente.

### Añadir con cámara o lector de códigos

Pulse **Cámara** desde la ficha, o **Escanear ISBN** desde Inicio.

- Autorice al navegador a usar la cámara cuando lo solicite.
- Mantenga el código de barras estable y bien iluminado frente a la cámara.
- Si el navegador reconoce el código, buscará el libro o abrirá una nueva ficha con el ISBN escrito.

También se puede conectar un lector USB de códigos de barras. Normalmente funciona como un teclado: haga clic en un campo ISBN, escanee el código y pulse la acción de consulta.

> La lectura con cámara depende del navegador y del permiso concedido. Si no está disponible, la aplicación muestra una alternativa clara: introducir el ISBN manualmente o usar un lector USB.

### Qué conviene rellenar

- **Colección:** dónde se agrupa el libro, por ejemplo “Biblioteca general” o “Juvenil”.
- **Ubicación:** lugar físico, por ejemplo `Sala principal · Estante B · Balda 2`.
- **Etiquetas:** palabras separadas por comas, como `poesía, siglo XX, autoras`.
- **Cantidad de copias:** número de ejemplares físicos que posee. Cada copia recibe un código interno.
- **Estado de las copias:** valoración general de conservación.

## 4. Consultar si se tiene un libro

Hay dos formas sencillas:

1. Escriba el título, autor o ISBN en el buscador superior.
2. Entre en **Catálogo** y use el filtro de búsqueda.

Cada libro muestra uno de estos estados:

| Estado | Significado |
| --- | --- |
| **Disponible** | Hay al menos una copia física que se puede consultar o prestar. |
| **Prestado** | Todas las copias están prestadas. |
| **Sin copias** | Existe la ficha bibliográfica, pero no hay ningún ejemplar físico registrado. |

Pulse cualquier portada o fila de libro para abrir su ficha completa. Allí aparecen ISBN, editorial, año, ubicación, etiquetas, notas y disponibilidad.

## 5. Organizar colecciones

Entre en **Colecciones** y pulse **Nueva colección**.

1. Escriba un nombre claro.
2. Añada una breve descripción opcional.
3. Pulse **Crear colección**.

Puede crear colecciones por ubicación (`Sala infantil`), uso (`Club de lectura`), temática (`Historia local`) o público (`Juvenil`). Al añadir o editar un libro, seleccione la colección correspondiente.

Al pulsar una tarjeta de colección se abre el catálogo filtrado por ella.

## 6. Registrar un préstamo

Puede hacerlo desde la ficha de un libro disponible, con el botón **Prestar una copia**, o desde **Préstamos** con **Registrar préstamo**.

1. Seleccione el libro y la copia que se va a prestar.
2. Escriba el nombre de la persona.
3. Añada teléfono o correo si resulta útil.
4. Indique la fecha de salida y la fecha prevista de devolución.
5. Puede guardar una nota, por ejemplo `Club de lectura de septiembre`.
6. Pulse **Confirmar préstamo**.

La copia cambiará automáticamente a estado **Prestado**. Si la fecha prevista ya ha pasado, el listado la marcará como **Vencido**.

### Devolver un libro

1. Abra **Préstamos**.
2. Localice la fila del préstamo.
3. Pulse **Devolver**.

La copia vuelve a estar disponible inmediatamente y el préstamo deja de aparecer entre los activos.

## 7. Revisar el inventario

Abra **Inventario** para ver cada ejemplar individual. Esta vista es especialmente útil para bibliotecas con varias copias del mismo libro.

La tabla muestra:

- Código interno de la copia.
- Libro al que pertenece.
- Ubicación física.
- Si está disponible o prestada.
- Estado de conservación.

Use esta sección al hacer un recuento, revisar estanterías o comprobar un ejemplar concreto.

## 8. Editar o eliminar una ficha

1. Abra la ficha del libro desde el catálogo.
2. Pulse **Editar ficha**.
3. Cambie los datos necesarios y pulse **Guardar libro**.

Para eliminar un libro, abra la edición y pulse **Eliminar**. Se pedirá confirmación porque también se eliminan sus copias y sus registros de préstamo asociados.

## 9. Exportar una copia de seguridad

Entre en **Datos y ajustes**. Hay dos formatos:

- **Descargar respaldo JSON:** conserva todo el catálogo, colecciones, copias, préstamos y ajustes. Es el formato recomendado para hacer una copia de seguridad o mover la aplicación a otro ordenador.
- **Exportar libros CSV:** crea una hoja de cálculo simple con los libros y sus campos principales. Es útil para consultar los datos en Excel, LibreOffice o Google Sheets.

Se recomienda descargar un respaldo JSON antes de realizar cambios importantes y, como mínimo, una vez al mes.

## 10. Importar datos

En **Datos y ajustes**, pulse **Elegir archivo**.

### Restaurar una copia de Estantería

Seleccione un archivo JSON exportado previamente por Estantería. Se restaurarán libros, colecciones, copias, préstamos y ajustes.

### Añadir libros desde un CSV

Puede importar un archivo CSV con una primera fila de encabezados. Los campos reconocidos son:

```text
title,author,isbn,year,publisher,collection,location,tags,copies
```

Ejemplo:

```csv
title,author,isbn,year,publisher,location,tags,copies
La casa de Bernarda Alba,Federico García Lorca,9788467045171,1936,Austral,Sala 1 · A2,teatro;clásico,2
```

Tras importar, revise algunas fichas para comprobar que las columnas se han interpretado correctamente.

> Al restaurar un JSON se sustituye el catálogo actual. Exporte un respaldo antes si desea conservarlo.

## 11. Borrar todos los datos

En **Datos y ajustes**, pulse **Borrar base de datos local** y confirme la acción.

Esto elimina el catálogo guardado en el navegador actual. No se puede deshacer. Descargue primero un respaldo JSON si existe la posibilidad de necesitar esos datos después.

## 12. Consejos prácticos

- Use una nomenclatura coherente para las ubicaciones: `Sala · Estante · Balda`.
- Cree etiquetas sencillas y repetibles; por ejemplo, use siempre `novela histórica` y no alternativamente `novela-histórica`.
- Para préstamos frecuentes, asigne a cada copia una ubicación y conserve visible su código interno.
- Haga una copia JSON antes de actualizar el navegador, limpiar sus datos o cambiar de equipo.
- Si varias personas van a utilizar la misma biblioteca, usen el mismo navegador/equipo o intercambien periódicamente el archivo de respaldo. Esta versión no sincroniza datos entre dispositivos por sí sola.

## 13. Privacidad y conexión

El catálogo y los préstamos se almacenan localmente en el navegador. La aplicación no requiere cuenta ni envía el catálogo a un servidor propio.

Solo al usar **Completar por ISBN** se consulta un servicio bibliográfico externo para obtener los datos de ese ISBN. El uso normal del catálogo, inventario, préstamos y respaldos funciona sin conexión una vez que la página está abierta.
