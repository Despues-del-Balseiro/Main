# Cómo contribuir

Gracias por sumar a la guía. Los aportes chicos cuentan: una fecha límite, un investigador o un párrafo de consejos ya sirven.

## Tres formas de contribuir

### 1. Completar un formulario (no hace falta saber usar GitHub)

Andá a **Issues → New issue** y elegí un formulario:

| Formulario | Sirve para |
|---|---|
| Agregar un lugar | sumar una universidad, un instituto, un programa o una empresa |
| Agregar una persona | sumar un investigador o un contacto en la industria |
| Contar tu historia | contar cómo te fue en tu búsqueda |
| Agregar una ciudad | contar cuánto cuesta vivir en una ciudad y cómo es el día a día |
| Sugerir un cambio | avisar que algo está desactualizado, está mal o falta |

Alguien del equipo de mantenimiento copia tus respuestas en el archivo que corresponde. Los issues los puede ver cualquiera que tenga acceso al repositorio.

### 2. Editar un archivo desde el navegador

Los nombres de los botones están en inglés, tal como aparecen en GitHub.

1. Abrí el archivo que quieras cambiar, por ejemplo `academia/materia-blanda/lugares.md`.
2. Hacé clic en el ícono del lápiz (✏️), arriba a la derecha del archivo.
3. En **Cómo agregar…**, abrí la plantilla, apretá el botón de copiar y pegala al final del archivo.
4. Completala usando la entrada de EJEMPLO como guía.
5. Hacé clic en **Commit changes…**. Si GitHub te pregunta, elegí **Create a new branch and start a pull request** y después **Propose changes**. Alguien del equipo de mantenimiento lo va a revisar.

**Para agregar tu historia:** andá a la carpeta `historias/` de tu área, hacé clic en **Add file → Create new file**, ponele de nombre `AAAA-nombre-apellido.md` (AAAA = el año en que te recibiste) y pegá la [plantilla de historia](plantillas/historia.md).

**Para agregar una ciudad:** seguí los pasos de [ciudades/](ciudades/). Si la ciudad ya tiene archivo, editá ese archivo en lugar de crear uno nuevo.

### 3. Usar Git

Cloná el repositorio, creá una rama, hacé commit y abrí un pull request. Un tema por pull request facilita la revisión.

## Reglas

### Sobre personas (investigadores y contactos)

- **Solo comentarios positivos.** Si tu experiencia no fue buena (incluido no recibir respuesta), dejá el campo de comentarios en blanco.
- **Un campo vacío no significa nada.** No lo leas como una advertencia, y no esquives la regla con indirectas como "sin comentarios".
- **Solo información pública y profesional:** nombre, institución, temas de investigación y un link a su página pública. No copies direcciones de mail ni datos personales.
- Si alguien ya está en la lista, no lo agregues de nuevo: sumá tu nombre en *Contactado/a por* y tu comentario en una línea nueva.
- Las mismas reglas valen para cualquier persona que menciones en tu historia.

### Sobre lugares y fechas límite

- Completá siempre **Agregado por / última revisión** con el mes y el año.
- Escribí el cierre *habitual* (por ejemplo, "todos los años a fines de noviembre") y también la fecha exacta, si la sabés. Las fechas exactas cambian; los patrones, en general, no.
- Poné un link a la página oficial en lugar de pegar el texto de la convocatoria.
- Si un lugar ya está en la lista, actualizá esa entrada en lugar de agregar una nueva.

### Sobre las historias

- Un archivo por persona. Si después querés agregar algo, editá tu propio archivo.
- Lo honesto sirve más que lo prolijo. *Qué haría distinto* suele ser la sección más valiosa.

### En general

- Escribí en español. Si preferís escribir en inglés, también vale.
- No borres las entradas de EJEMPLO: le muestran el formato a quien llega por primera vez.

## Markdown en un minuto

| Escribís | Obtenés |
|---|---|
| `### Nombre` | un título (usá uno por entrada) |
| `- ítem` | una viñeta |
| `**negrita**` | **negrita** |
| `[texto](https://example.org)` | un link |
| una línea vacía | un párrafo nuevo |

## Agregar un área nueva

Si tu área no está (física médica, información cuántica, astrofísica, …), cualquier persona con permiso de escritura en el repositorio la puede crear en un minuto:

1. Andá a la pestaña **Actions** y elegí **Agregar área** en la lista de la izquierda.
2. Hacé clic en **Run workflow**, escribí el nombre del área tal como querés que se vea (por ejemplo, *Física médica*) y, si querés, los temas que incluye.
3. Hacé clic en el botón verde **Run workflow**.

En menos de un minuto aparece la carpeta nueva en `academia/`, con sus archivos y entradas de EJEMPLO, y el área se suma a la tabla de [academia/README.md](academia/README.md), a los formularios y a [general/encuesta.md](general/encuesta.md). Lo único que queda a mano es agregarla como opción en la pregunta *Área* de la encuesta de Google Forms.

Si no tenés permiso de escritura, abrí un issue de *Sugerir un cambio* y alguien del equipo de mantenimiento la crea.
