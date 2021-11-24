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
| RF003 | **Módulo de publicidad** | 18/09/21 | Alto |
| **Descripción** | En este módulo el cliente tendrá la posibilidad de visualizar los diferentes productos disponibles, podrá observar foto, descripción, precio, y disponibilidad. |
| **Entradas** | **Fuente** | **Salida** | **Destino** | 
|-Barra de búsqueda -Seleccionar filtros por categorías de productos o servicios | Base de datos| Detalles y descripción de productos y ofertas -Cantidad disponible | Vista previa de productos y ofertas |
| **Restricciones** | Solo se puede hacer pedido si se ha iniciado sesión en el sistema |
|**Proceso**| Ingresar a la URL del sistema > Visualizar todos los productos > Hacer búsqueda por nombre de producto específico > Filtrar por categoría o fecha de publicación > Seleccionar producto > Vista previa. |
| **Efecto colateral** | - No puede conocer los productos a detalle - No puede hacer pedidos|


| Código | Nombre | Fecha | Grado necesidad |
| --- | --- | --- | --- | 
| RF009 | **Gestión de Información (CRUD)** | 03/10/21 | Alto |
| **Descripción** | En este módulo de gestión de información, los miembros administrativos tendrán la posibilidad de crear, leer, actualizar y borrar toda la información (productos, servicios, clientes, trabajadores, pedidos, proveedores) en el aplicativo web |
| **Entradas** | **Fuente** | **Salida** | **Destino** | 
|Información de datos del sistema de información (productos, clientes, proveedores, pedidos)| Formulario de gestión de información (productos, clientes, proveedores, pedidos) | Menú principal de administrador | Base de datos |
| **Restricciones** | Si no ingresa como usuario administrador, no podrá acceder a este módulo |
|**Proceso**| > Dirigirse al menú principal > Clic en gestión de información > Escoger información a gestionar (productos, clientes, proveedores, pedidos) > Escoger opción (crear, leer, actualizar, eliminar) |
| **Efecto colateral** | No podrá tener gestionar la información (productos, clientes, proveedores, pedidos)| 



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

