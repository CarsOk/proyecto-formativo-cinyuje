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
