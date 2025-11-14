# 05 — Integración con Gmail (OAuth GCP + Add-on)

- En opciones en la parte de abajo vamos a activar la opcion de plugin de correo
![](../assets/img/05-integracion_gmail/plugins.png)


- Desde el correo, vamos a buscar a la aplicacion de odoo inbox admin, y vamos a iniciar sesion
![](../assets/img/05-integracion_gmail/inbox.png)


- Aqui hay una comprobación de que odoo está instalado en el gmail
![](../assets/img/05-integracion_gmail/comprobacion.png)


- Ahora en ajustes tenemos que darle a autentificacion oauth y guardar
![ ](../assets/img/05-integracion_gmail/autenticacionOauth.png)


- Despues le damos a proveedores oauth y sale esta pestaña
![ ](../assets/img/05-integracion_gmail/proveedoresOauth.png)


- Ahora vamos a entrar en la pagina de proyecto en cloud para vincular el gmail
![](../assets/img/05-integracion_gmail/proyectoCloud.png)


- Una vez dentro vamos a buscar la API de gmail
![](../assets/img/05-integracion_gmail/buscadorAPI.png)


- Una vez la hayamos encontrado, elegimos nuestro proyecto
![](../assets/img/05-integracion_gmail/continuarAPI.png)


- Despues vamos a darle al boton de credenciales de la derecha, y deberia de abrirse una pestaña como esta, y vamos a darle a datos de usuario, y continuamos
![](../assets/img/05-integracion_gmail/credencialesUsuario.png)


- Ahora ponemos el nombre de nuestro proyecto, nuestro correo electronico y el correo de contacto con el desarollador (puede ser el mismo)
![](../assets/img/05-integracion_gmail/credencialesUsuario.png)


- Si continuamos al paso 3 podemos elegir los permisos, hay que marcar los que tengo
![](../assets/img/05-integracion_gmail/permisos.png)


- Para el cuarto paso hay que elegir "Aplicacion Web" y poner tu url de redireccionamiento, que seria "https://usuario.odoo.com/google_gmail/confirm"
![](../assets/img/05-integracion_gmail/idCliente.png)


- Ahora tenemos que ir a las credenciales y entrar en nuestro proyecto
![](../assets/img/05-integracion_gmail/irACredenciales.png)


- Y aqui tendriamos todos nuestros datos
![](../assets/img/05-integracion_gmail/datos.png)


- Por ultimo vamos a copiar el ID del cliente y vamos a pegarlo en la pestaña que estabamos en odoo, activamos el "permitido" e iniciamos sesion en google
![](../assets/img/05-integracion_gmail/copiarID.png)

- Ahora si le damos a la opcion en ajustes de utilizar servidores de correo electronico personalizados, nos sale una pestaña nueva, ahí copiamos el ID, y el secreto
![](../assets/img/05-integracion_gmail/servidorCorreo.png)


