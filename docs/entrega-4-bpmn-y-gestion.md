# Entrega 4 - Modelado de Procesos, Gestion Agil y Control del Sistema.

# 1. Resumen.

En esta cuarta entrega se consolidaron los análisis realizados en las entregas anteriores mediante el modelado del proceso de negocio que el software automatizará.
Se elaboró un diagrama BPMN del proceso de registro de venta y actualización automática de stock, incluyendo pools, lanes, tareas, eventos, compuertas lógicas y excepciones.
El proceso involucra al cliente, vendedor, sistema de gestión, depósito, administración y proveedor.
Además, se documentó el proyecto en un repositorio público de GitHub, se organizaron las historias de usuario en un tablero ágil y se definieron indicadores de control 
y estándares de desempeño para auditar el funcionamiento del sistema. 
Finalmente, se incluyó la declaración de uso de inteligencia artificial, explicando su función de apoyo y las correcciones realizadas.

# 2. Introduccion.

En las entregas anteriores se analizó a TecnoFácil S.R.L. como una organización empresarial y sistema abierto, se realizó un análisis estratégico mediante FODA 
y se definió su estructura organizacional, junto con un sistema de información orientado a ventas, productos, stock, usuarios y reportes.
Esta cuarta entrega consolida el proyecto mediante el modelado del proceso de negocio que el software automatizará, la organización del trabajo en un repositorio Git/GitHub,
la gestión del backlog ágil y la definición de indicadores de control para auditar el desempeño del sistema. 
El objetivo es demostrar que la propuesta no se limita a una idea de software, sino que se integra con los procesos, roles y necesidades de información de la empresa.

# 3. Objetivos.

Modelar en BPMN el proceso de venta y actualización de stock de TecnoFácil S.R.L.
Representar los actores internos, externos y el comportamiento automatizado del sistema.
Documentar el proyecto en un repositorio público de GitHub con control de versiones.
Gestionar las historias de usuario mediante un tablero ágil.
Definir indicadores y estándares para auditar el funcionamiento del sistema.
Declarar de forma transparente el uso de inteligencia artificial en la elaboración del trabajo.

# Modelado de Procesos de Negocio — BPMN
# Proceso modelado:
El proceso modelado es “Registro de venta y actualización automática de stock”.
El sistema permitirá consultar la disponibilidad de productos, validar los datos de la venta, descontar automáticamente el stock, generar comprobantes y emitir alertas cuando un producto alcance su stock mínimo.

# 1.2 Pools y Lanes:
Pool:                      Lane:                   Responsabilidad:
TecnoFacil S.R.L           Cliente                 Solicita un producto y recibe la mercadería.
TecnoFacil S.R.L           Vendedor                Atiende al cliente, consulta stock y registra la venta.
TecnoFacil S.R.L           Sistema de Gestión      Valida stock, registra la venta, descuenta stock y emite comprobante.
TecnoFacil S.R.L           Depósito                Prepara y entrega el producto.
TecnoFacil S.R.L           Administración          Controla ventas, cobros y reportes.
Proveedor                  Proveedor               Recibe pedidos de reposición y entrega mercadería.

# Flujo estándar:
El cliente solicita un producto.
El vendedor consulta la disponibilidad en el sistema.
El sistema verifica el stock disponible.
Si hay stock, el vendedor registra la venta.
El sistema valida los datos del cliente, producto, cantidad y precio.
El sistema descuenta automáticamente la cantidad vendida del stock.
El sistema genera el comprobante de venta.
El depósito prepara y entrega el producto.
El sistema registra la entrega y actualiza el estado de la venta.
Administración consulta reportes de ventas, stock y facturación.

# Compuertas lógicas y excepciones:
Compuerta:                  Decisión:                                 Camino normal:               Excepción:
Gateway exclusiva XOR       Hay stock disponible?                     Si: continúa la venta.       No: se informa falta de stock y se genera pedido de reposición.
Gateway exclusiva XOR       Los datos de la venta son válidos?        Si: se confirma la venta.    No: el sistema solicita corrección al vendedor.
Gateway exclusiva XOR       El stock quedó por debajo del mínimo?     No: finaliza el proceso.     Si: se genera alerta y pedido sugerido a Compras.


# 4. Conclusion.

Esta entrega integra el análisis organizacional realizado en las instancias previas con herramientas de modelado, colaboración y gestión ágil. 
El diagrama BPMN permite comprender cómo el sistema de TecnoFácil S.R.L. automatizará el proceso de venta, control de stock y generación de información.
El uso de GitHub permite documentar el proyecto, controlar las versiones y evidenciar el trabajo colaborativo mediante ramas, commits y Pull Requests. 
Por su parte, el tablero ágil facilita el seguimiento de las historias de usuario y de sus estados.
Finalmente, los indicadores de control permiten auditar el desempeño del sistema y verificar si este contribuye a reducir errores, mejorar la trazabilidad, 
evitar faltantes de stock y facilitar la toma de decisiones.
