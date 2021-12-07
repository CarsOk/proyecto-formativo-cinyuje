# Especificación de requerimientos

## Introducción

El propósito del SRS es documentar los requisitos del sistema de información y los acuerdos a los que se lleguen entre el cliente y el equipo de desarrollo. Estos requisitos son indispensables para el desarrollo del sistema de información , estos se hacen para dejar claramente los requerimientos y necesidades establecidos por el cliente, este documento estará firmado por el cliente y el equipo de desarrollo, lo plasmado en este documento será lo que se llevará a cabo y se deberá cumplir por los analistas.


## Propósito

El propósito del SRS es dejar documentado los acuerdos que se lleven entre el cliente y los analistas, en este proyecto formativo se diseñara, desarrollara e implementara un aplicativo web que cumpla con los requerimientos y especificaciones dadas por el cliente. Este SRS servirá como control para verificar la ejecución e implementación del sistema de información, que al cumplirse estas, ayudará a llevar un control de ventas e inventario en la microempresa cinyuje, una vez terminado el aplicativo web estará listo para ponerlo en marcha, este sistema de información estará desarrollado por el equipo de desarrollo (aprendices).


## Alcance

El alcance de este proyecto será la creación de un aplicativo web que permitirá a los usuarios, tener mejor acceso a la información de la empresa, su inventario y ventas. Dentro de los módulos que tendrá el sistema de información, en este caso un aplicativo web, serán: 

* Módulo de acceso al sistema (login)

* Módulo dedicado al registro de usuarios (clientes)

* Módulo de publicidad

* Módulo de pedidos

* Módulo manejo de inventario


## Definiciones, Acrónimos, y Abreviaturas

* SRS: Es un documento donde se realizan las especificaciones de los requerimientos o requisitos del software. En esta documentación se muestran los acuerdos a los que se llegaron el grupo de desarrollo y el cliente.

* Mapa de procesos: Un mapa de procesos es un diagrama que permite ver de forma gráfica y organizada, todos los procesos que se llevan a cabo dentro de una organización y sus interrelaciones. 

* Diagrama de flujo: Es un gráfico utilizado para representar la serie de actividades que se presentan o llevan a cabo en un proceso. Este mejora la comprensión del mismo, muestra sus relaciones e incidencias.

* Sistema de información: es un conjunto de componentes interrelacionados los cuales están compuestos por elementos sociales, técnicos y organizados para recolectar, procesar, ordenar, almacenar y convertir datos en información.

* Aplicativo web: es un conjunto de páginas web que se adaptan para que varios usuarios puedan acceder a través de un servidor usando internet, por medio del navegador.

* Desarrollador: un desarrollador es un programador. Se encarga de brindar soluciones para la creación de programas o aplicativos web. Estos tienen como deber, escribir y mantener el código. 


## Referencias

Universidad ICESI.  (2010, 15 de Octubre). SRS / ERS Especificación de requerimientos de software.
https://www.icesi.edu.co/departamentos/tecnologias_informacion_comunicaciones/proyectos/lisa/home/analisis/srs/srs
	
Myriam Quiroa (2021, 04 de Enero). Mapa de procesos. Economipedia.com
https://economipedia.com/definiciones/mapa-de-procesos.html

Conexionesan (2019, 12 de Noviembre). El uso del diagrama de flujo para la gestión de calidad https://www.esan.edu.pe/apuntes-empresariales/2019/11/el-uso-del-diagrama-de-flujo-para-la-gestion-de-calidad/
	
(Laudon & Laudon, 2012; Piccoli, 2012)
	
Euroinnova Business School. (S.f). APRENDE LA DEFINICIÓN DE PROGRAMADOR DE COMPUTADORAS Y DE QUÉ TRATA ESTA INTERESANTE PROFESIÓN
https://www.euroinnova.co/blog/definicion-de-programador

https://www.crehana.com/co/blog/desarrollo-web/aplicacion-web-que-es/


## Atencion y Dependencia

| Área | Sistema Software donde va actuar |
| ---- | ---- |
| Administrativa | En esta área el sistema va funcionar donde el gerente o dueño va tener acceso a todos los módulos  software  hacer pedidos,  comprar la materia prima, el registro de usuarios y mostrar los productos de la microempresa. |
| Operativa | Aquí el sistema actuara con todo lo relacionado con inventario, ubicación de productos y de la materia prima |
| Atencion al cliente | El software procesa toda solicitud del cliente y sus necesidades con relación a los productos promoción para que los clientes de la microempresa puedan hacer sus pedidos |
| Despacho | En esta área la persona se apoya en el sistema para el alistamiento del producto  y para la entrega al cliente cuantos productos salen. |


## Requerimientos Específicos


### Requerimientos Funcionales


| Código | Nombre | Fecha | Grado necesidad |
| --- | --- | --- | --- | 
| RF001 | **Inicio de sesión** | 18/09/21 | Alto |
| **Descripción** | En este módulo los usuarios podrán iniciar sesión con correo electrónico y contraseña. Contará con botón de “Ingresar”. Y tendrán la opción de recuperar la contraseña. |
| **Entradas** | **Fuente** | **Salida** | **Destino** | 
|- Correo electrónico - Contraseña | Base de datos | - Nombre completo - Foto de perfil | Menú principal, página de promoción.|
| **Restricciones** | El usuario no podrá tener acceso al sistema y sus funcionalidades si no se registra e inicia sesión.|
|**Proceso**| Digitar correo electrónico y contraseña > Clic en botón “ingresar” > Verificación en la base de datos. Si los datos son correctos, se realiza el ingreso. De lo contrario, se muestra un mensaje al usuario, pidiendo que por favor verifique la información e intente nuevamente.> Si el usuario olvidó su contraseña de acceso, dará clic en “recuperar contraseña”.  En la misma interfaz se solicitará ingresar número de identificación, y correo electrónico. >  Una vez digite la información de manera correcta, se enviará detalles de recuperación.|
| **Efecto colateral** | El usuario no podrá ingresar al sistema, no podrá tener acceso a todas las funcionalidades para realizar pedidos, Bloqueo por intentos fallidos, Cierre de sesión automático | 


| Código | Nombre | Fecha | Grado necesidad |
| --- | --- | --- | --- | 
| RF002 | **Registro de cliente y usuario** | 18/09/21 | Alto |
| **Descripción** | En este módulo el cliente y/o usuario tendrán la posibilidad de registrarse en el aplicativo web |
| **Entradas** | **Fuente** | **Salida** | **Destino** |
| - Identificación -Fecha de nacimiento -Nombres y apellidos -Correo electrónico -Contraseña -Contacto telefónico -Celular -Dirección -Rol | Formulario de registro de cliente | Mensaje de confirmación | -Base de datos -Página de promoción de productos ofertas y descuentos |
| **Restricciones** | El cliente no podrá escoger su rol o perfil en sistema, a diferencia del administrador. -Debe completar toda la información el usuario que no se encuentre registrado en el sistema |
| **Proceso** |  Clic en el botón registro de cliente o usuario > Diligenciar el formulario registro de usuario > Diligenciar el formulario registro de cliente > Clic en el botón “Registrar” > Acceder a la página de oferta y promoción |
| **Efecto colateral** | -	Mensaje de error > No puede ingresar al sistema > El cliente solo puede acceder al módulo promociones |


| Código | Nombre | Fecha | Grado necesidad |
| --- | --- | --- | --- | 
| RF003 | **Módulo de publicidad** | 18/09/21 | Alto |
| **Descripción** | En este módulo el cliente tendrá la posibilidad de visualizar los diferentes productos disponibles, podrá observar foto, descripción, precio, y disponibilidad. |
| **Entradas** | **Fuente** | **Salida** | **Destino** | 
|-Barra de búsqueda -Seleccionar filtros por categorías de productos o servicios | Base de datos| Detalles y descripción de productos y ofertas -Cantidad disponible | Vista previa de productos y ofertas |
| **Restricciones** | Solo se puede hacer pedido si se ha iniciado sesión en el sistema |
|**Proceso**| Ingresar a la URL del sistema > Visualizar todos los productos > Hacer búsqueda por nombre de producto específico > Filtrar por categoría o fecha de publicación > Seleccionar producto > Vista previa. |
| **Efecto colateral** | - No puede conocer los productos a detalle - No puede hacer pedidos|


| Código | Nombre | Fecha | Grado necesidad |
| --- | --- | --- | --- |
| RF004 | **Módulo de pedidos** | 18/09/21 | Alto |
| **Descripción** | Este módulo permitirá ver al cliente los pedidos realizados, que productos están en la cesta o carrito de compras. Con este módulo puede gestionar (crear, editar, borrar, listar) sus pedidos el cliente |
| **Entradas** | **Fuente** | **Salida** | **Destino** |
| -Resumen de pedido -Códigos o referencias -Precio de los productos -Disponibilidad de producto | Base de datos pedidos realizados | Productos seleccionados, disponibilidad de producto | -Vista de los artículos seleccionados -Reporte detallado sobre el pedido |
| **Restricciones** | Solo pueden finalizar y visualizar el pedido los usuarios registrados |
|**Proceso**| -Buscar la página de la empresa, Iniciar sesión -Seleccionar los productos, El sistema verifica la disponibilidad de producto -Escoger productos para el pedido, Vista de todos los pedidos seleccionados, Le notificara por un mensaje en pantalla que se acerque al punto de la empresa a hacer el pago |
| **Efecto colateral** | No puede hacer los pedidos si no está registrado  > El pedido no podrá ser despachado si no está pagado, se debe acercar a las oficinas para hacer el pago y se elabore su pedido |


| Código | Nombre | Fecha | Grado necesidad |
| --- | --- | --- | --- |
| RF005 | **Módulo de administrador** | 05/10/2021 | Alto |
| **Descripción** | En este módulo el administrador podrá gestionar y tener acceso a los módulos del sistema (inventario, consulta, pedidos, gestión, ayuda, etc.) para gestionar toda la información del aplicativo web |
| **Entradas** | **Fuente** | **Salida** | **Destino** |
| - Inicio de sesión  - Contraseña - Correo electrónico - Foto de usuario  - Perfil | Información de la base de datos | - Inicio de sesión,  Contraseña > Correo electrónico > Foto de usuario,   Perfil | - Inventario > Pedidos > Ayudas, Gestión de información > Consulta > PQRS |
| **Restricciones** | Solo el administrador puede acceder a este módulo |
| **Proceso** | >	Módulo de administrador >	Clic en el módulo a dirigirse >	Lo llevará al módulo que se haya seleccionado |
| **Efecto colateral** |  Si no es administrador no podrá acceder |


| Código | Nombre | Fecha | Grado necesidad |
| --- | --- | --- | --- | 
| RF006 | **Módulo de Manejo de Inventario** | 30/09/21 | Alto |
| **Descripción** | Este módulo permitirá llevar un control de inventarios de cada uno de los productos por su descripción, referencia, precio, cantidad, stock disponible y así mismo este arroje un mensaje de notificación donde muestre cuántos productos hay en existencia y cuántos se han vendido. |
| **Entradas** | **Fuente** | **Salida** | **Destino** |
| Lista de productos > Código del producto | Base de datos | Inventario del Producto •ID •Descripción •Referencia •Precio | •Stock Disponible •Existencias Iniciales •Cantidad Comprada •Cantidad de Pedidos •Cantidad Vendida | 
| **Restricciones** | El administrador y el encargado del área de despachos podrán acceder y tener información del inventario de la microempresa. |
|**Proceso**| • Clic Botón  • Lista de Productos • Ingrese el Código del Producto  • Base de Datos • Inventario del Producto • ID del Producto • Descripción • Referencia • Precio • Stock Disponible • Cantidad Existentes • Existencias Iniciales • Cantidad Comprada • Cantidad Vendida |
| **Efecto colateral** | No puede acceder al stock de inventarios para obtener información detallada de los productos, sólo los trabajadores que estén registrados en el sistema o quien haga las veces del encargado. |


| Código | Nombre | Fecha | Grado necesidad |
| --- | --- | --- | --- | 
| RF007 | **Módulo de PQRS** | 30/09/21 | Alto |
| **Descripción** | Este módulo permite al usuario realizar peticiones, quejas, reclamos y sugerencias |
| **Entradas** | **Fuente** | **Salida** | **Destino** | 
|Correo electrónico contraseña| Formulario de PQRS |Se comunicaría con un encargado| Base de datos o correo electrónico al administrador |
| **Restricciones** | Solo los usuarios registrados tendrán acceso a el módulo de PQRS |
|**Proceso**| Inicio de sesión > Dirigirse a la parte inferior de la página > Seleccionar la opción de PQRS > Escribir la sugerencia o el problema > Esperar la respuesta. |
| **Efecto colateral** | Solo clientes registrados podrán hacer solicitud de PQRS - Solo el administrador podrá ver estas solicitudes |


| Código | Nombre | Fecha | Grado necesidad |
| --- | --- | --- | --- | 
| RF008 | **Módulo de consulta** | 3/10/21 | Alto |
| **Descripción** | Este módulo permitirá a los trabajadores y administrador consultar y tener reportes toda la información del aplicativo web |
| **Entradas** | **Fuente** | **Salida** | **Destino** |
| Búsqueda de información (usuarios, proveedores, pedidos, fecha de entrega, estado del pedido, reportes del sistema en general) | Información de la base de datos (tablas) | Información solicitada de la consulta | Interfaz de la consulta realizada | 
| **Restricciones** | Solo pueden visualizar la información usuarios como trabajadores y administrador |
| **Proceso** | 	Iniciar sesión  >	Ir a consulta > 	Filtrar por información >   	Clic en consultar >	Botón de reporte >  	Imprimir reporte de la consulta | 
| **Efecto colateral** | Si no hay información sobre lo consultado mostrará un mensaje que no se ha encontrado información que coincida con la búsqueda |


| Código | Nombre | Fecha | Grado necesidad |
| --- | --- | --- | --- | 
| RF009 | **Gestión de Información (CRUD)** | 03/10/21 | Alto |
| **Descripción** | En este módulo de gestión de información, los miembros administrativos tendrán la posibilidad de crear, leer, actualizar y borrar toda la información (productos, servicios, clientes, trabajadores, pedidos, proveedores) en el aplicativo web |
| **Entradas** | **Fuente** | **Salida** | **Destino** | 
|Información de datos del sistema de información (productos, clientes, proveedores, pedidos)| Formulario de gestión de información (productos, clientes, proveedores, pedidos) | Menú principal de administrador | Base de datos |
| **Restricciones** | Si no ingresa como usuario administrador, no podrá acceder a este módulo |
|**Proceso**| > Dirigirse al menú principal > Clic en gestión de información > Escoger información a gestionar (productos, clientes, proveedores, pedidos) > Escoger opción (crear, leer, actualizar, eliminar) |
| **Efecto colateral** | No podrá tener gestionar la información (productos, clientes, proveedores, pedidos)| 

| Código | Nombre | Fecha | Grado necesidad |
| --- | --- | --- | --- | 
| RF010 | **Módulo de Ayuda** | 05/10/21 | Alto |
| **Descripción** | Se visualizará una ayuda para saber cómo hacer uso de las funcionalidades del sistema (inicio de sesión, registro de clientes, usuarios, inventario, gestión de información, consulta y pedidos)  |
| **Entradas** | **Fuente** | **Salida** | **Destino** | 
|Selección del cliente(inicio de sesión, registro de clientes, usuarios, inventario, gestión de información, consulta y pedidos) |   Base de datos |PDF | Interfaz con la información de ayuda requerida|
| **Restricciones** | Ninguna |
|**Proceso**|  Clic botón de ayuda (signo de interrogación) > Menú con nombres de módulos > Clic en el módulo en el que requiere ayuda > Interfaz de información del módulo requerido para la guía del proceso|
| **Efecto colateral** | Ninguno |


### Requerimientos no funcionales 

| Código | Nombre | Fecha | Grado necesidad |
| --- | --- | --- | --- | 
| RNF001 | **Desempeño** | 18/09/21 | Alto |
| **Descripción** | El aplicativo web debe contar con un excelente rendimiento. El tiempo de carga debe ser máximo de cinco segundos. |



| Código | Nombre | Fecha | Grado necesidad |
| --- | --- | --- | --- | 
| RNF002 | **Confidencialidad** | 18/09/21 | Alto |
| **Descripción** | Se debe garantizar la seguridad de los datos ingresados por los usuarios, haciendo cumplir la ley 1266 de 2008 (habeas data) |



| Código | Nombre | Fecha | Grado necesidad |
| --- | --- | --- | --- | 
| RNF003 | **Seguridad** | 23/09/21 | Alto |
| **Descripción** | Es de suma importancia porque es algo que prima en todo sistema de información. Es por esto que para aplicarlo, se hará uso de una contraseña y correo electrónico con lo que cada usuario podrá tener su información segura dentro del sistema |

### Requerimientos de interfaz de usuario


| Código | Nombre | Fecha | Grado necesidad |
| --- | --- | --- | --- | 
| RI001 | **Interfaz de inicio de sesión** | 29/09/21 | Alto |
| **Descripción** | La interfaz de inicio de sesión va a permitir al usuario acceder al sistema y hacer uso de sus funcionalidades, ingreso al menú principal, y la acción de realizar pedidos.Una vez el usuario ingresa al aplicativo web, podrá visualizar el botón de inicio de sesión en la parte superior derecha. Si se encuentra registrado, dará clic en iniciar sesión y visualizará la interfaz. La interfaz contará con espacios donde se solicitará al usuario digitar correo electrónico y contraseña, estos datos deben ser iguales a los que este digitó en su registro. En caso contrario, al hacer clic en el botón “iniciar sesión” saldrá un mensaje que dirá “(correo electrónico o contraseña) incorrecto/a. Por favor verifique la información e intente nuevamente". En caso de que el usuario olvide su contraseña, en la misma interfaz se contará con una opción llamada “recuperar contraseña”. Al hacer clic, al usuario se le pedirá digitar número de identificación y correo electrónico. Una vez añadida la información, podrá hacer clic en el botón enviar. Si la información coincide, al usuario se le enviará la información que le permitirá volver a acceder al aplicativo. Se mostrará el mensaje “Sus datos se han restablecido correctamente. Revise su correo electrónico.” Al cliente le llegará la información vía correo electrónico para restablecer su contraseña. Si los datos digitados por el cliente no son los correctos, se mostrará un mensaje indicando que la información añadida no es correcta, y este no podrá ingresar al sistema.|


| Código | Nombre | Fecha | Grado necesidad |
| --- | --- | --- | --- | 
| RI003 | **Interfaz de publicidad** | 29/09/21 | Alto |
| **Descripción** | En la interfaz de publicidad, el cliente tendrá la posibilidad de visualizar los diferentes productos disponibles; podrá observar su foto, descripción, precio, y disponibilidad. La interfaz de publicidad podrá ser visualizada una vez el cliente haga ingreso al aplicativo. En esta, tendrá la posibilidad de ver todos los productos y servicios ofrecidos. Podrá ver fácilmente cada uno de ellos y comparar entre sus diferentes características para que así pueda hacer su mejor elección. Existirá una barra donde podrá escribir para realizar búsqueda de productos específicos, teniendo la alternativa de conseguirlos por nombres, filtros de categoría o fecha de publicación  y de esta manera,  poder ver lo más reciente. Si el producto ingresado en la barra de búsqueda no existe en la base de datos, se mostrará un mensaje indicando que el producto no existe. Si existe, el cliente tendrá la posibilidad de seleccionar productos, que los dirigirá a la interfaz de pedidos.|


| Código | Nombre | Fecha | Grado necesidad |
| --- | --- | --- | --- | 
| RI005 | **Interfaz de PQRS** | 04/10/21 | Alto |
| **Descripción** |En esta interfaz de PQRS, el cliente entrara a la página de la microempresa después ingresa su usuario y contraseña. Irá al menú del cliente, le dará clic en parte inferior donde se encuentra el botón de PQRS, en ese momento le desplegará un formulario de PQRS donde colocará su nombre completo, identificación, fecha y la petición queja sugerencia y reclamo que tenga el cliente. Por último, le dará clic en enviar formulario. Le saldrá un mensaje “enviado correctamente” de lo contrario le saldrá error si no está lleno un campo obligatorio.|


| Código | Nombre | Fecha | Grado necesidad |
| --- | --- | --- | --- | 
| RI009 | **Interfaz de Gestión de Información (CRUD)** | 04/10/21 | Alto |
| **Descripción** | En esta interfaz el administrador podrá crear, actualizar o borrar información de clientes, trabajadores, productos y servicios de eventos. Donde el administrador ingresa a la página de la microempresa por medio de una url, después ingresa su usuario y contraseña y ahí lo dirige al menú principal. Después, le dará clic en el botón gestión de información, se desplegará un menú con varias opciones de información de productos, de clientes, trabajadores y servicios de eventos, donde podrá modificar crear y actualizar todos estos datos.|
