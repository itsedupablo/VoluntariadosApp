# VoluntariadosApp
**Falla la DB de firebase y no me deja añadir voluntariados. Intentaré solucionarlo a ver si me da tiempo. Lo demás en teoría es funcional.**
### Enlace al repositorio: https://github.com/itsedupablo/VoluntariadosApp
## Descripción
VoluntariadoApp es una aplicación Android que permite gestionar voluntariados. Los usuarios pueden ver voluntariados disponibles, apuntarse a ellos y, en algunos casos, agregar nuevos voluntariados a la plataforma. La app está diseñada para ser simple y fácil de usar, con la integración de Firebase para el manejo de la autenticación de usuarios y almacenamiento de datos.

## Características
Autenticación de Usuario: Los usuarios pueden registrarse e iniciar sesión utilizando Firebase Authentication.
Ver Voluntariados: Los voluntariados disponibles se muestran en una lista, y los usuarios pueden consultar detalles sobre cada uno.
Agregar Voluntariados: Los usuarios pueden agregar nuevos voluntariados a la plataforma si lo desean.
Apuntarse a Voluntariados: Los usuarios pueden apuntarse a los voluntariados disponibles.
Base de Datos Firebase: La aplicación utiliza Firebase Realtime Database para almacenar la información de los voluntariados y las inscripciones de los usuarios.
## Estructura de la Aplicación
La aplicación se organiza en las siguientes partes:

- MainActivity: Actividad principal que muestra la lista de voluntariados disponibles. Se relaciona también con los **Fragments** AgregarVoluntatariado, ListaVoluntariados y DetallesVoluntariados
- AgregarVoluntariadoFragment: Fragmento que permite agregar un nuevo voluntariado a la base de datos de Firebase.
- VoluntariadoAdapter: Adaptador de RecyclerView que gestiona la visualización de los voluntariados en una lista.
- Voluntariado: Clase modelo que representa los voluntariados y contiene los atributos como nombre, descripción, fechas, etc.
- MyApplication: Clase de aplicación que inicializa Firebase al arrancar la aplicación.
- SplashActivity: Clase para mostrar el icono personalizado de la app al inicio
- AccessActivity: Clase que permite al usuario registrarse y hacer login en la app
## Uso
- Iniciar sesión: Los usuarios pueden iniciar sesión utilizando su correo y contraseña.
- Agregar voluntariados: Después de iniciar sesión, los usuarios pueden agregar nuevos voluntariados mediante un formulario que incluye campos como nombre, ubicación, fechas de inicio y fin, etc.
- Ver voluntariados disponibles: Los voluntariados que se han añadido aparecerán en la lista principal.
- Apuntarse a un voluntariado: Los usuarios pueden inscribirse en voluntariados disponibles manteniendo presionado un elemento de la lista y seleccionando la opción "Apuntarse".
