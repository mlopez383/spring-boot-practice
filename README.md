#Project Statement

Realizar una plataforma e-learning donde se puedan impartir cursos online similares a Udemy, Coursera o PluralSight.

##Requirements
A web application that allows us to perform the following operations:
Sign Up - Sign In - Sign Out - User Configuration
1.The web application will have the following roles:

**Administrator:** Es el rol responsable de la plataforma, con las siguientes funcionalidades:
- Gestionar los  cursos (Listar,  agregar, modificar o eliminar un curso).
- La opción  de  “Loguearse Como” y seleccionar cualquier usuario del sistema para navegar la plataforma como si fuese el mismo.
- Envío de e-mail a un estudiante, a los estudiantes de un curso o bien a un instructor.
- Puede editar su perfil personal.
- Envío masivos de mensajes a diferentes roles de la plataforma, como ser a los instructores o estudiantes.
- Como administrador del sitio, podrá ingresar a los foros y modificar o eliminar comentarios.   
- Puede  dar  de  alta  cursos,  configurarlos  y también crear y asignar lecciones y  exámenes a los mismos.

**Estudiante:** es  quien podrá  sumarse a un curso que tenga  disponible  y  gestionar  su  perfil.  El  mismo podrá:
- Comenzar cualquier curso que tenga disponible en el catálogo de cursos.
- Ver el grado de avance en los cursos que esté tomando.
- Acceder  al  contenido  del  curso  que  el  instructor publique.
- Realizar los cuestionarios que el instructor publique.
- Acceder a sus certificados de cursos finalizados.
- Modificar su perfil personal.
- Podrá darle un puntaje al curso realizado.
- Ver un reporte de los cursos realizados (listado con el nombre del curso, fecha de inicio y fecha de finalización).
- Participar de un foro del curso que esté tomando con el instructor y compañeros de curso.
- Enviar mensajes por medio de la plataforma.

**Instructor:** es quien generará los contenidos del curso. El mismo podrá:
- Modificar la información personal de su perfil.
- Tendrá un dashboard general, donde podrá ver y acceder a editar los cursos que el mismo tiene.
- Podrá ver desde el dashboard las últimas consultas recibidas por alumnos.
- El alta del curso  se realizará mediante lecciones  que  quedarán asociadas  a un  contenido, por  ejemplo  “Cómo  redactar  emails  correctamente” sería  el título  de la lección y luego debería  de poder  cargar un  contenido de  texto con formato, asociarse fotos, videos,  tablas, links, etc.
- Podrá  responder  mensajes  a  consultas  de alumnos  o realizar consultas  al administrador del sitio, por consultas técnicas, etc.
- Puede dar de alta, modificar, eliminar preguntas de evaluación.

##Create and publish course
3. The application allows users with the instructor role to create courses. The instructor must enter the following information to create a course:
- Course name.
- Description
- Category
- Price
- Course evaluation (This is not entered by the Instructor, it has to be taken from evaluations made by students).
- Videos: The system must allow the uploading of videos.
- Images: The system must allow the uploading of images.
- Content: The system must allow the uploading of contents.
- Files: The system must allow the uploading of files (PDF, DOC, XML).

4. The course has two states active and inactive. The instructor can activate it. A course in active status is displayed in search results.
5. The instructor can edit a course, delete it as long as it is not active. If you want to modify or delete it, you must first deactivate it.

## Search and view courses
6. Users with the Student role have the possibility to search for courses using different types of filters:
- Course name.
- Category
- Price range

7. The search result should show the courses that match the user's search.

## Curso en Promoción
8. El sistema contará con una característica llamada Curso en Promoción. La promoción consiste en que el curso más antiguo que esté activo en el sistema entra a promoción para los posibles estudiantes. La promoción consiste en que el usuario que acceda de primero al curso obtendrá un 50% de descuento. El sistema debe dar como máximo 10 minutos al usuario para registrarse en el curso. Si este tiempo pasa, el curso se libera y otro estudiante puede acceder a él. Para este feature específico, Ud debe utilizar programación concurrente. La opción Curso en Promoción sólo puede ser activada por el usuario administrador del sistema.