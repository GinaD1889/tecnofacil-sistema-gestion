# Entrega 2 - Analisis Estrategico y Planificacion del Sistema

# Resumen.

En esta segunda entrega se evaluó la viabilidad del proyecto de software para TecnoFácil S.R.L. mediante un análisis FODA enfocado en los recursos, capacidades y 
condiciones del entorno.
Se definieron el objetivo general, las metas cuantitativas y los resultados esperados del sistema. Además, se aplicaron conceptos de la Teoría General de Sistemas, 
como sinergia, homeostasis, entropía y retroalimentación, para analizar el impacto del software en la organización.
También se describió la arquitectura técnica propuesta, con sus módulos de ventas, productos, stock, usuarios y reportes, y se elaboró un diagrama de Gantt para 
planificar las tareas, plazos, dependencias y responsables del desarrollo.

# Introduccion.

En la primera entrega se analizó a TecnoFacil SRL como un sistema abierto y se propuso desarrollar un módulo integrado de inventario y ventas. 
En esta segunda etapa se evaluará la viabilidad del proyecto, se definirán sus objetivos y metas, y se organizará un cronograma de desarrollo. 
Además, el análisis incorpora propiedades de la Teoría General de Sistemas, como la sinergia, la homeostasis, la entropía y la retroalimentación. 
También se detallarán aspectos técnicos de la solución propuesta, especialmente su arquitectura, sus módulos principales y la forma en que intercambiará información 
con las distintas áreas de la empresa.

# Objetivos.

Evaluar la viabilidad del proyecto software mediante una matriz FODA. 
Definir el objetivo general y las metas cuantitativas del sistema. 
Aplicar conceptos de la TGS. 
Describir la arquitectura técnica del software. 
Planificar el desarrollo mediante un diagrama de Gantt. 

# Análisis FODA del proyecto: 
El Análisis FODA se enfoca exclusivamente en la viabilidad y el desarrollo del módulo de software propuesto. Por lo tanto, las fortalezas y debilidades corresponden
principalmente al equipo técnico y a los recursos disponibles, mientras que las oportunidades y amenazas representan factores externos del mercado y del entorno organizacional. 

# Relación con la TGS: 
Fallas de conectividad, hardware o servidores. 
Resistencia del personal a modificar sus procedimientos. 
Riesgos de acceso no autorizado o pérdida de información. 
Cambios tecnológicos que vuelven obsoletas algunas herramientas. 
El proyecto puede analizarse como una intervención sobre un sistema abierto. La incorporación del software busca producir sinergia, ya que la integración entre inventario, 
ventas, compras y administración permitirá obtener mejores resultados que los que lograría cada área trabajando con información aislada. 
También se espera contribuir a la homeostasis de la organización, porque el sistema facilitara la adaptación ante cambios en la demanda, los precios, el stock y las condiciones de los 
proveedores. A su vez, permitirá disminuir la entropía, entendida como el desorden producido por registros duplicados, información desactualizada, errores de carga o falta de 
comunicación entre sectores. 
Finalmente, los reportes, alertas y opiniones de los usuarios funcionaran como mecanismos de retroalimentación, permitiendo corregir errores y ajustar el funcionamiento del sistema. 

# Objetivos y Metas: 
# Objetivo general: 
Desarrollar e implementar un módulo integrado de inventario y ventas para TecnoFacil SRL que permita centralizar la información, actualizar el stock en tiempo real y mejorar la 
coordinación entre las áreas de ventas, deposito, compras, facturacion y administracion. 
El sistema deberá contribuir a reducir la entropía organizacional mediante la eliminación de registros duplicados y la actualización automática de la información. Asimismo, buscará 
generar sinergia entre las distintas áreas al permitir que todos los sectores autorizados trabajen con datos consistentes. 

# Metas cuantitativas: 
● Finalizar una primera versión funcional del sistema en un plazo máximo de 12 semanas. 
● Registrar y migrar el 100% del catálogo activo de productos antes de la implementación. 
● Lograr que la consulta de stock tenga un tiempo de respuesta máximo de 2 segundos. 
● Reducir en un 80% los errores de registro de stock durante los primeros tres meses. 
● Capacitar al 100% de los usuarios antes de la puesta en producción. 
● Permitir el almacenamiento de al menos 10.000 productos y 50.000 operaciones de venta. 
● Alcanzar una disponibilidad mínima del sistema del 98% durante el horario comercial.                                                 
● Obtener al menos un 85% de aceptación por parte de los usuarios durante la evaluación piloto. 

# Enfoque técnico y Arquitectura del software: 
# Arquitectura propuesta: 
Se propone una arquitectura de tres capas, compuesta por presentación, lógica de negocio y datos. Este modelo separa la interfaz utilizada por los usuarios, las reglas que controlan el 
funcionamiento y la información almacenada en la base de datos.

# Componentes principales: 
# Capa de presentación: 
Permitirá: 
● Iniciar sesión según el tipo de usuario. 
● Registrar y consultar productos. 
● Consultar stock disponible. 
● Registrar ventas. 
● Visualizar alertas de stock mínimo. 
● Consultar reportes básicos.

# Capa de lógica de negocio: 
Será responsable de:  
● Validar los datos ingresados. 
● Impedir ventas sin stock disponible. 
● Descontar automáticamente los productos vendidos. 
● Generar alertas de reposición. 
● Calcular totales de venta. 
● Controlar permisos de usuarios. 
● Registrar cada movimiento de inventario.

La separación por capas favorece la modularidad, facilita el mantenimiento y permite modificar una parte del sistema sin alterar completamente las demás. 

# Tecnologías posibles: 
● Interfaz: HTML, CSS  y JavaScript. 
● Servidor: Python con Flask o Django. 
● Base de datos: SQLite para el prototipo y PostgreSQL para una versión ampliada. 
● Comunicación: API REST. 
● Control de versiones: Git. 
● Seguridad: Usuarios, roles, validación de entradas y contraseñas protegidas. 
● Respaldo: Copias de seguridad periódicas.

# Planificación temporal: 
El diagrama de Gantt permite visualizar las tareas, sus duraciones, responsables, 
dependencias y fechas de ejecución.  
Las actividades se ordenan considerando que algunas requieren la finalización previa de 
otras. 
Responsables: 
● CO: coordinador del proyecto. 
● AF: analista funcional. 
● DT: diseñador técnico. 
● DP: desarrollador. 
● QA: responsable de calidad. 
● RU: representante de los usuarios de TecnoFacil SRL. 

# Conclusión: 
El análisis realizado permite considerar viable el desarrollo del módulo de inventario y ventas para TecnoFacil SRL, siempre que se controle el alcance, se capacite a los usuarios y se 
implementen medidas de seguridad y respaldo. La propuesta técnica de tres capas favorece la organización y el mantenimiento del sistema, mientras que la planificación temporal ordena 
las tareas según sus dependencias. Desde la perspectiva de la TGS, el software no constituye una solución aislada, sino una 
intervención que modifica las relaciones entre los subsistemas de la empresa. Su incorporación busca generar sinergia, mantener la estabilidad operativa, reducir la entropía y utilizar 
la retroalimentación para mejorar continuamente el funcionamiento organizacional. 
