# Diseño estructural I: Teoría de las estructuras

Todos los archivos van juntos en la raíz del repositorio, sin carpetas.

Sitio del curso PROF00806 (Universidad UTE, período 2026-II, martes y jueves de 09:00 a 11:00). Docente: Francisco Javier Almeida Navarrete. Tiene tres páginas:

| Página | Para quién | Qué hace |
|---|---|---|
| `index.html` | Estudiantes | Logo de la UTE, fecha y hora, franja con tres ilustraciones que cambian cada segundo, próxima actividad (con «empieza en…» o «en curso»), línea del semestre, cronograma, lecturas, contacto con el docente (WhatsApp, teléfono y correo), **reserva de tutorías**, ponderación de la evaluación y lista personal de tareas |
| `asistencia.html` | Estudiantes | Cada estudiante escribe sus **nombres y apellidos completos** y genera su QR de asistencia, que lleva también la **fecha y la hora** en que lo generó; esos datos se ven debajo del código |
| `clase.html` | Docente | **Modo clase** en la laptop o el proyector: sesión del día, temporizador y avance del semestre |
| `registro.html` | Docente | **Registro de asistencia** en una pestaña aparte: la lista con número, nombres y apellidos (✓ verde presente, ✗ roja falta), marcar tocando o escaneando QR (cámara en vivo o foto) y enviar el Excel de cada sesión a su correo |

Este sitio **complementa** el Aula Virtual (Moodle). No recibe entregas ni registra calificaciones, y el registro oficial de asistencia sigue siendo el de la Universidad UTE.

## Cómo registrar la asistencia

**Una sola vez, al inicio del semestre**

1. Abra `registro.html` en la laptop que usará en clase (Chrome o Edge, desde la dirección https de GitHub Pages).
2. La lista del curso (22 estudiantes, en orden alfabético) está en `lista-curso.js` y se carga sola. Para cambiarla, edite ese archivo en GitHub y cambie `LISTA_VERSION` (por ejemplo, a la fecha de hoy): al abrir el registro, la lista del navegador se reemplaza y la asistencia ya registrada pasa a cada estudiante según su nombre, aunque cambie su número. **Ojo:** el repositorio es público, así que esos nombres los puede ver cualquiera.
3. Si usará QR, envíe por WhatsApp el enlace `https://SU-USUARIO.github.io/diseno-estructural-i/asistencia.html`. En cada clase, el estudiante pulsa «Generar mi código»: sus nombres quedan guardados en el teléfono y el QR lleva la fecha y la hora del momento.

**En cada clase**

1. En el modo clase, pulse **Registrar asistencia**: se abre el registro de la sesión del día en una pestaña nueva.
2. Marque a los presentes de cualquiera de estas formas (se pueden combinar):
   - **Tocando al estudiante:** ✓ verde es presente; otro toque lo quita (✗ roja, falta).
   - **Marcar todos presentes** y luego tocar a quien no vino.
   - **Escanear QR:** se abre la cámara en vivo (en GitHub Pages). Si la cámara no se enciende, como ocurre dentro del visor de Claude, use **Tomar foto del QR**: en el celular abre la cámara del teléfono y el registro lee la foto. Con la cámara en vivo, cada estudiante acerca su teléfono y aparece su número y nombre con un tono. El sitio reconoce el nombre aunque el estudiante lo haya escrito incompleto o sin tildes, y **le avisa en amarillo si el código no se generó hoy** (por ejemplo, la captura de un compañero). Si hay dudas (por ejemplo, dos estudiantes con el mismo apellido), le pregunta a usted, y el caso queda en **Por resolver** para decidir después, sin frenar la fila. Después de la primera vez, cada QR se reconoce solo por su código.
3. Compare el nombre de la pantalla con la persona que tiene delante.
4. **Al terminar, pulse «Enviar Excel a mi correo».**
   - En Windows se abre el panel **Compartir** con el Excel ya adjunto: elija Outlook o Correo y envíelo a su dirección.
   - Si su navegador no tiene esa opción, el Excel se descarga y se abre un correo listo, dirigido a majid.khorami@ute.edu.ec: solo arrastre el archivo descargado al correo.
   - El registro muestra «Aún no envió el Excel de esta sesión» hasta que lo haga, y lo avisa de nuevo si cambia algo después.

Una página web publicada en GitHub Pages no puede enviar correos por sí sola sin un servidor; por eso el envío pasa por su programa de correo, en un solo paso.

**El Excel de cada sesión** (`Asistencia_PROF00806_S06_2026-10-22.xlsx`) tiene dos hojas:
- **Sesión:** los estudiantes en orden de lista (alfabético), con Presente o Falta, hora y forma de registro (QR o manual), más presentes, faltas y porcentaje calculados con fórmulas de Excel.
- **Semestre:** una columna P/F por cada sesión registrada, con asistencias, sesiones y porcentaje de cada estudiante, y los presentes por sesión.

**Importante sobre los datos**

- La lista y la asistencia se guardan **solo en el navegador de la laptop** donde se registran. Si se borran los datos de ese navegador, se pierde lo no enviado.
- Para cambiar de computadora, use **Más opciones → Descargar respaldo completo** y luego **Restaurar un respaldo** en la nueva. Restaurar no duplica registros.
- La asistencia es un dato personal de los estudiantes: guarde los Excel según la normativa de la UTE y no los suba a este repositorio. El registro oficial de asistencia sigue siendo el de la Universidad UTE.

## Fotos, entregas y enlaces

- **Franja de fotos:** `foto-1.jpg` a `foto-7.jpg` (fotos de estructuras, recortadas y comprimidas). Se muestran tres a la vez en pantallas anchas y una en el celular, y cambian cada 3 segundos; el botón «Pausar fotos» las detiene. Para cambiar una foto, reemplace el archivo con el mismo nombre.
- **Entrega del trabajo autónomo:** siempre en la siguiente clase, una hora antes de que empiece (08:00). Se calcula sola con el cronograma; cada tarea muestra «Vence hoy», «Faltan N días» o «Plazo vencido».
- **Aula Virtual (Moodle):** botón azul debajo de «Mi código QR de asistencia», que abre https://lms.ute.edu.ec/login/.
- **Correo:** el botón «Correo (Outlook)» y el envío de solicitudes de tutoría abren Outlook en la web (correo UTE) con el mensaje listo.

## Tutorías

El horario de tutorías aún no está definido: la sección «Contacto y tutorías» muestra el correo del docente. Cuando haya horario, complete `tutorias` en `silabo.json` (`dia`, `inicio`, `fin`, `modalidad`, `lugar`, `reserva`) y se activará el botón **Reservar una tutoría**.

## Fechas del curso

El sílabo no trae fechas. Las 32 sesiones se asignaron en orden a los martes y jueves desde el 6/10/2026 (sesión 1), sin el feriado del 3/11, las vacaciones del 21/12 al 1/1 ni el carnaval (9/2). Así quedan el **Parcial 1 el 24/11** (sesión 14), el **Parcial 2 el 26/1** (sesión 28) y el **Examen final el 4/2** (sesión 31). Si el calendario académico fija otras fechas, cámbielas en `silabo.json`.

## Cómo actualizar una fecha, un tema o un enlace

Todo el contenido del curso está en `silabo.json`. El diseño (los archivos `.html`, `.css` y `.js`) no se toca durante el semestre.

1. En GitHub, abra `silabo.json` y pulse el ícono del lápiz (Edit this file).
2. Cambie solo el texto entre comillas. Por ejemplo, para mover el Parcial 1, busque `"2026-11-24"` en la sección `sesiones` y escriba la nueva fecha con el mismo formato (año-mes-día).
3. Actualice también `"actualizado"` con la fecha de hoy.
4. Pulse **Commit changes**. El sitio se actualiza solo en uno o dos minutos.

Si la página dice que no pudo leer el cronograma, probablemente falta una coma o unas comillas en el último cambio.

## Probar otra fecha

Agregue `?hoy=AAAA-MM-DD` a la dirección de `index.html`, `clase.html` o `registro.html`, por ejemplo `registro.html?hoy=2026-11-19`.

## Privacidad

El repositorio es público: todo lo que se sube aquí, incluido su historial, lo puede ver cualquiera. El sitio no envía datos a ningún servidor. Las bibliotecas de QR están incluidas en `` (ver `LICENCIAS.md`) y no se cargan de internet. El Excel se genera en el propio navegador con `xlsx-mini.js`, sin servicios externos.
