# angular-project

# Proyecto: Application Full-stack: Capa de presentación

### Introducción

Empezamos a construir una **aplicación full-stack**. Comenzaremos por la parte de presentación utilizando el framework de desarrollo de Angular.

El trabajo se puede desarrollar de forma **individual** o en **pareja**.

Empieza el trabajo esbozando los **wireframes** (borradores) y las **user stories** (historias de usuario), antes de empezar a meter código. 

### Requisitos funcionales y técnicos de alto nivel:
- **La aplicación tendrá al menos 2 modelos(clases o interfaces)** que representen:
  + Al usuario
  + A la entidad principal objeto de la aplicación.
- **Tendrá las funcionalidades de registro / login / logout**, con token de acceso y flujo de autorización (conexión a la Api).
- **Tendrá todas las rutas CRUD** de al menos uno de los modelos.
- **Será Responsive**. Recomendación: Comienza diseñando para pantallas pequeñas y luego para las grandes.
- **Se desplegará en un servidor de hosting**  

### Requisitos técnicos de bajo nivel:

1. Elementos que deberá incluir la aplicación:
- Un directorio de elementos comunes **shared** con la siguiente estructura:
  + Un directorio **services** con **al menos 2 servicios**:
    - Uno para autenticación: `AuthService`
    - Uno para conexión a la API: `ApiService`

  + Un directorio **guards**:
    -  Con **el guard**: `AuthGuard`  

- Un módulo **CommonsModule** con los elementos comunes a la aplicación:
  + Pantalla Inicial: `HomeComponent`
  + Barra de Navegación: `NavBarComponent`
  + Pantalla 404: `NotfoundComponent`
  + [Opcionales] `HeaderComponent`, `FooterComponent`, `AsideComponent`, ...  

- Un módulo **UserModule** que contendrá, **al menos**, los componentes:
  + Listado de usuarios: `UserListComponent`
  + Detalle de usuario: `UserComponent`
  + Formulario de registro de usuario: `RegisterComponent`
  + Formulario de login de usuario: `LoginComponent`

- Un módulo por cada unidad funcional de la aplicación. **[NombreEntidad]Module** con los componentes mínimos:
  + Listado de elementos: `[Nombre]ListComponent`
  + Detalle del elemento: `[Nombre]Component`
  + Formulario alta de elemento: `[Nombre]FormComponent` 

2. La aplicación incluirá un elemento de enrutamiento a nivel de root (`RoutingModule`) y opcionalmente enrutamiento a nivel de módulos funcionales.

3. La aplicación debe incluir conexión a una API, puedes utilizar la utilidad [json-server](https://github.com/typicode/json-server) y [json-auth-server](https://www.npmjs.com/package/json-server-auth), o cualquier otra alternativa con los siguientes endpoints:
   1. Funcionalidad principal:
      1. listado general
      2. traer un único elemento
      3. Crear elemento
      4. Borrar elemento
   2. Usuarios
      1. Register
      2. Login
 

### Entregables

1. **Wireframes de la aplicación** foto/escaneado de papel, pizarra, etc. o archivo de alguna herramienta como [Sketch](https://www.sketchapp.com/).
2. **Presentación del proyecto**, con [slides.com](http://www.slides.com).
3. **Front-end de la aplicación hecha en Angular** y hospedada en algún servidor.
4. **link a la aplicación** en la sección URL del repositorio GitHub.
5. **Un archivo ``readme.md``** con explicación de las tecnologías usadas, la estrategia de desarrollo utilizada, instrucciones de instalación, problemas no resueltos, etc.
6. **Repositorio Git en Github**, con enlace al proyecto desplegado. La aplicación tendra un readme.md con toda la información a entregar.

---

### Sugerencias

* **Comienza con la idea final en mente.** Planifica con borradores e historias de usuario las tareas que vas a realizar. No pierdas tiempo en hacer cosas que no necesitas.
* **Escribe código basura, si lo necesitas, para resolver algún problema a corto plazo**. Con la idea de refactorizarlo antes de ponerlo en producción.
* **Lee la documentación de cualquier tecnología que emplees.** La mayor parte de las veces hay algún tutorial que seguir, pero no siempre, y aprendenr a leer documentación es crucial para tener éxito como desarrollador.
* **Commit early, commit often.** (haz commit pronto y a menudo) No temas romper algo porque siempre tendrás una versión anterior a la que volver.
* **Las historias de usuario definen el tipo de usuario al que se quiere llegar con la aplicación**. Es tentador hacer listas _todo_ de todo lo que habría que hacer, pero si defines tareas pequeñas y focalizadas en lo que importa al usuario, desde su perspectiva, te ayudará a saber qué es lo que quieres construir.
* **Escribe seudocódigo antes del código.** Pensar en la lógica de algo ayuda a estructurar el código final.
* **Haz tuyo cualquier código que encuentres.** Huye del copy-paste de ejemplos. Refactorízalo y escríbelo, quédate con la idea no con el código. 

---

### Ideas de proyectos:

##### Gestión Comercial gamificada

Desarrolla la aplicación comercial que gestione un stock de productos. Implementa un motor que vaya consumiendo el stock y obligue a adquirir más stock.


##### Bookmarket

Crea una aplicación para crear marcadores de enlaces que los usuarios quieran mantener.
Los usuarios pueden vender los enlaces o compartirlos o...lo que se te ocurra.

##### Custom Travel Agency

Sé tu propia agencia de viajes. Customiza tus viajes en función de la información que otros viajeros han compartido. El formato es en forma de guía de viajes. La aplicación da la plantilla y los usuarios la completan. A la hora de montar un viaje consiste en juntar todos los *booklets* que después se puedan imprimir.

---

### Enlaces útiles

* **[Heroku](http://www.heroku.com)**, [CDmon](https://www.cdmon.com/es/)
* **[Writing Good User Stories](http://www.mariaemerson.com/user-stories/)** _(Algunas ideas para escribir historias de usuario)_
* **[Presenting Information Architecture](http://webstyleguide.com/wsg3/3-information-architecture/4-presenting-information.html)** _(Una visión de los wireframes)_

---

### Feedback y evaluación


* __Requisitos técnicos__: Has entregado un proyecto que cumple los requerimientos técnicos?  

* __Creatividad__: Has añadido algún elemento creativo, spinner personal, etc.? Has entregado algo que enganche o que pueda ser "jugable" al usuario?

* __Calidad del Código__: Has seguido las buenas prácticas que han ido saliendo en clase, diseño modular, nombres semánticos,...?

* __Despliegue__: Has desplegado la aplicación?

* __Total__:

    Puntuación | Expectativas
    ----- | ------------
    **0** | _No cumple las expectativas_
    **1** | _Cumple las expectativas, buen trabajo!_
    **2** | _Excede las expectativas, eres un(a) crack!_

## Esquema de la presentación 

### Formato

- Duración de la presentación: 6 minutos
- Q & A: 3 minutos
- **Tiempo Total:** 9 minutos

### Qué mostrar 
- una presentación con [slides.com](https://slides.com/)
- Una demo con GitHub pages
- La presentación y la demostración debe ser ejecutable en cualquier servidor

### Qué decir
- Corta presentación sobre ti:
	- Quién eres?
	- Algún hobby que tengas
  - __Ahora la presentación__
- Elevator pitch:
  - Qué app quieres construir
  - Por qué la has elegido
  - La característica más importante de la app
- Algún reto técnico que te hayas tenido que resolver:
  - plantéalo
  - explica como lo has resuelto
  - muestra y explica trozos de código en la presentación
- Tecnologías que has usado:
  - Alguna librería que hayas instalado
- Git:
  - Muestra un pantallazo con los commits que hayas hecho
- Product Demo:
  - Muestra alguna historia de usuario (ej: como un usuario utilizará la app)
  - Demuestra la característica importante de tu app
  - Rápidamente, pasa por otras características de la app
- Algún error que hayas cometido:
  - Has cometido errores en la planificación del tiempo? planteando el objetivo? conceptualizando la aplicación? Programando?
