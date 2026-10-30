# Resumen.

En esta tercera entrega se definió la estructura formal de TecnoFácil S.R.L. mediante un organigrama piramidal vertical.
Se identificaron la Gerencia General como máximo nivel de autoridad y las áreas de Administración y Finanzas, Área Comercial y Ventas, y Operaciones y Abastecimiento. 
También se describieron las funciones principales de cada área y su relación con el sistema de información propuesto.
Asimismo, se elaboró un diccionario de datos preliminar con las entidades Producto, Venta y Usuario, definiendo sus campos, tipos de datos y funciones dentro del sistema. 
Esta entrega vincula la estructura organizacional con los datos y procesos que deberá administrar el software.

# Introduccion.

En las dos primeras entregas se realizó un análisis general de TecnoFácil S.R.L., considerando sus características, actividades principales y necesidades de información. 
También se estudió la importancia de implementar un sistema que permita integrar y mejorar los procesos relacionados con las ventas, los productos, el control de stock y la generación 
de reportes.  A partir de ese análisis, se identificaron los principales usuarios y sectores involucrados, como Vendedores, Depósito, Compras y Administración. Además, se planteó 
una arquitectura del sistema organizada en capas, compuesta por la capa de presentación, la lógica de negocio y la capa de datos.  
En esta tercera entrega se profundizará en la organización formal de la empresa y en la estructura inicial de la información que utilizará el sistema. Para ello, se elaborará un 
organigrama piramidal vertical que represente los niveles jerárquicos y las relaciones de autoridad, junto con un diccionario de datos preliminar que describa las entidades y los 
campos fundamentales del negocio. El diccionario permitirá establecer un lenguaje común y evitar interpretaciones diferentes sobre los datos del sistema. 

# Objetivos.

● Diseñar la estructura jerárquica formal de TecnoFácil S.R.L.  
● Identificar las unidades organizacionales más importantes de la empresa.  
● Representar correctamente las relaciones de autoridad y asesoramiento.  
● Elaborar un diccionario de datos preliminar.  
● Describir los campos principales de cada entidad.

# Funciones principales:  
● Gerencia General: establece objetivos, toma decisiones estratégicas y supervisa el funcionamiento general.  
● Administración y Finanzas: controla documentación, pagos, cobranzas, registros y resultados económicos.  
● Área Comercial y Ventas: atiende clientes, registra ventas y realiza el seguimiento comercial. 
● Operaciones y Abastecimiento: controla el inventario, el depósito y la reposición de productos.  
● Depósito y Stock: recibe, almacena y entrega productos, además de actualizar las existencias.  
● Compras y Proveedores: solicita cotizaciones, realiza pedidos y mantiene la relación con proveedores.  
● Área de Sistemas: administra el sistema de información, usuarios, permisos, datos y reportes. 

# Entidad 1: Producto.
Esta entidad permite administrar el catálogo de productos y controlar las existencias. 
El campo stockActual se modifica cuando se registra una venta, una compra o un movimiento de depósito.  

# Entidad 2: Venta.
La entidad Venta registra cada operación comercial. 
Se relaciona con Usuario porque permite identificar quién cargó la venta y con Producto porque cada venta debe incluir uno o más productos. 

# Entidad 3: Usuario. 
La entidad Usuario permite controlar el acceso al sistema y asignar permisos según el puesto. 
Por ejemplo, un vendedor puede registrar ventas, mientras que un usuario de Administración puede consultar reportes y modificar información administrativa.  

# Conclusion.
La realización de esta tercera entrega permitió relacionar la estructura organizacional de TecnoFácil S.R.L. con las necesidades del sistema de información propuesto. 
El organigrama muestra cómo se distribuye la autoridad, qué áreas forman parte de la empresa y cómo se organizan las responsabilidades entre los distintos niveles jerárquicos.  
A su vez, el diccionario de datos permitió identificar la información esencial para el funcionamiento del sistema, especialmente aquella vinculada con los productos, las 
ventas y los usuarios. La definición de los campos y sus tipos facilita una futura construcción ordenada y coherente de la base de datos.  
En conclusión, esta entrega representa un avance en la planificación integral de la empresa, porque vincula la organización formal con los procesos y datos que deberán 
ser administrados. Una estructura jerárquica clara y un sistema de información correctamente definido contribuirán a mejorar el control del stock, el registro de 
ventas, la gestión de usuarios y la generación de reportes para la toma de decisiones. 
