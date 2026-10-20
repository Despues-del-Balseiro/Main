# Mantenimiento

Notas para quienes cuidan el repositorio. Conviene que haya al menos dos personas a cargo, de camadas distintas, para que la guía sobreviva a cada graduación.

## Configuración inicial

1. **Creá una organización en GitHub** (alcanza con el plan gratuito), por ejemplo `egresados-balseiro`. Un repositorio dentro de una organización no depende de la cuenta de una sola persona. Agregá a dos o tres personas como *owners*.
2. **Creá el repositorio** dentro de la organización y elegí su visibilidad:
   - *Público*: cualquiera puede leerlo y los futuros estudiantes lo encuentran fácilmente.
   - *Privado*: solo pueden leerlo los miembros invitados, así que hay que invitar a cada camada nueva.
3. **Subí los archivos.** Con Git, desde la carpeta descomprimida:
   ```bash
   git init -b main
   git add .
   git commit -m "Estructura inicial"
   git remote add origin https://github.com/ORGANIZACION/REPOSITORIO.git
   git push -u origin main
   ```
   Sin Git, usá **Add file → Upload files** y arrastrá el contenido de la carpeta. Después verificá que se haya subido la carpeta `.github`: algunos sistemas ocultan las carpetas cuyo nombre empieza con un punto, y sin ella no aparecen los formularios.
4. **Creá las etiquetas** que usan los formularios (**Issues → Labels → New label**): `sugerencia`, `nuevo-lugar`, `nueva-persona`, `nueva-historia`, `nueva-ciudad`.
5. **Creá la encuesta** en Google Forms con las preguntas de [general/encuesta.md](general/encuesta.md). Desactivá la opción de recopilar direcciones de correo electrónico. Reemplazá `LINK_ENCUESTA` en [README.md](README.md) y en [general/encuesta.md](general/encuesta.md) por el link del formulario.
6. *Opcional:* activá **Discussions** (Settings → General → Features) para preguntas abiertas que no encajan en un issue.

## Trabajo habitual

- **De formularios a archivos.** Cuando alguien envía un formulario, copiá el contenido en el archivo que corresponde usando la plantilla de ese archivo. Después cerrá el issue con un link al commit.
- **Revisá los pull requests**, sobre todo la regla sobre personas: los comentarios tienen que ser positivos o estar en blanco. Si no lo son, pedile a quien los escribió que los saque antes de aceptar el cambio. Lo mismo con las historias que mencionan a personas.
- **Áreas nuevas.** Usá **Actions → Agregar área → Run workflow** (los pasos están en *Agregar un área nueva*, en [CONTRIBUTING.md](CONTRIBUTING.md)). Crea la carpeta y actualiza la tabla de [academia/README.md](academia/README.md), los formularios y [general/encuesta.md](general/encuesta.md). Después sumá el área a mano en la pregunta *Área* del formulario de Google.
  - Si la acción falla al guardar los cambios con un error de permisos (403), andá a **Settings → Actions → General → Workflow permissions**, elegí **Read and write permissions** y volvé a correrla.
  - Si te equivocaste en el nombre, alguien que use Git lo puede deshacer con `git revert` sobre el commit "Agregar área: …". Sin Git: borrá los archivos de la carpeta creada (en cada archivo, menú **⋯ → Delete file**) y sacá el área de `academia/README.md`, de los tres formularios y de `general/encuesta.md`. Después corré la acción de nuevo con el nombre correcto.

## Todos los años (por ejemplo, al empezar el ciclo lectivo)

- Resumí la encuesta en [general/cuando-empezar.md](general/cuando-empezar.md).
- Marcá con `⚠️ revisar` las entradas cuya *última revisión* tenga más de un año.
- Traspaso: sumá al menos a una persona de la camada nueva y actualizá la tabla de abajo.

## Equipo actual

| Nombre | Usuario de GitHub | Camada |
|---|---|---|
| Luciano Lopez | LucianoLopezib | IB23 |
| | | |
| | | |
| | | |
