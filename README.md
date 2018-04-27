# Actividad_9
### 9º Actividad semanal. Ya tenemos todas las especificaciones de nuestra web app ahora vamos sólo tenemos que rematar y ampliar las rutas para que pueda servir con una api rest información para futuras aplicaciones móviles
Bueno pues ya tenemos nuetra web completamente activa y funcional, ahora vamos a simplemente abrir unas nuevas rutas para que puedan servirse viajes, login de usuario de tal manera que una aplicación móvil pueda alimentarse de la misma.

---
### Condiciones
Tenemos que generar una nueva ruta /api del cual se dispondrá diversos endpoints:
/api/user/login -> Endpoint donde se logueará nuestro usuario
/api/viajes -> Endpoint donde se recivirá todos los viajes.
/api/viajes/?:id -> Endpoint donde se recibirá el viaje indicado en la id.
  
---
## Características.
* Se utilizará NPM para la instalación de dependencias.
* El proyecto debe estar subido en un contendor en vagrant, y debe cumplir las siguientes condiciones:
  * Debe disponer de un vagrantfile y un archivo .sh donde se encuentren todos los scripts necesarios para construir el contenedor y nuestra aplicacion se autoejecute.
  * El contendor debe tener abierto el puerto 80 y apuntara internamente al puerto 3000 donde tenemos apuntado nuestro servidor de node.js
  * El contendor debe disponer un mysql instalado con la tabla descrita anteriormente.
  * Dentro del package.json debemos disponer la tarea production debe llamar al módulo forever y arrancar la maquina.
  * Debemos generar una nueva carpeta en nuestra estructura denominada log, donde se almacenará un log de los posibles errores que se produzcan en la aplicación.
  * Se utilizará nodemailer para el envio de los emails de los diferentes procesos.
  * Se utilizará Multer para las subidas de archivos al servidor.
  * Se utilizará sequelize para gestionar todas las entidades de nuestro proyecto como ORM del mismo.
  * Las vistas con las tablas dispondrán de paginación.
  * La gestión de las estrategias de logueo se realizará mediante passport.
  * Los permisos se gestionarán mediante JWT(Json Web Token).
