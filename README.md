# Mi Data Fabric

#### Objetivo
Este proyecto es un data fabric a pequeña escala que da prioridad a la ciberseguridad de los datos.

#### Funcionamiento del Sistema
Este proyecto se trabajó en jupyter notebook, [aquí](data_fabric.ipynb).
Al correr la función iniciar_sesion() en la celda [9], se pide al usuario su nombre, si este está listado en el registro de usuarios, se ofrecerá llenar las características de los datos a los que se desea acceder. Para esto, el usuario debe saber de antemano el nombre de la base de datos y columnas a las que se quiere acceder, esto con el fin de no revelar información adicional a la que el usuario no tiene nivel de acceso. Si el usuario cuenta con el nivel de seguridad requerida para acceder a la información solicitada, se le otorgará.

Simultaneamente se está llevando registro de todas las acciones y la hora y día en que fueron realizadas. En caso de que un usuario extraño intente ingresar al sistema sin un nombre de usuario válido, también se tomará registro. Las posibles acciones son las siguientes:

 - Log in.
 - Log out.
 - Unable to log in.
 - Request granted.
 - Request denied.
 - Invalid request.
Cabe mencionar que en el caso de "Invalid request." no se le hace saber al usuario, pero sí se toma registro de ello.
