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
Cliente                    Cliente                 Solicita un producto, realiza el pago y recibe la mercadería y el comprobante.
TecnoFacil S.R.L           Vendedor                Atiende al cliente, consulta stock, registra la venta y prepara/entrega el pedido.
TecnoFacil S.R.L           Sistema de Gestión      Valida los datos, descuenta el stock, actualiza el registro de ventas y evalúa el stock mínimo.
TecnoFacil S.R.L           Depósito                Verifica el stock físico, gestiona la reposición y recibe/actualiza la mercadería.
TecnoFacil S.R.L           Administración          Registra el pago, emite el comprobante y genera reportes de ventas y stock.
Proveedor Externo          Proveedor               Recibe la solicitud de reposición, prepara y envía la mercadería, y confirma el envío.

# Flujo estándar:
1. El cliente solicita el producto y el vendedor consulta su disponibilidad.
2. La compuerta exclusiva “¿Stock disponible?” deriva el flujo: con stock, se registra la venta; sin stock, se
informa la falta y se inicia la reposición.
3. En la venta normal, el Sistema de Gestión valida los datos, descuenta las unidades vendidas y actualiza el
registro.
4. El vendedor prepara el pedido y el Depósito entrega el producto al cliente.
5. Administración registra el pago, emite el comprobante y actualiza el reporte de ventas y stock.
6. La compuerta “¿Stock bajo mínimo?” evalúa el inventario. Si corresponde, Depósito genera una solicitud de
reposición al proveedor; si no, continúa el flujo normal.
7. El proveedor recibe la solicitud, prepara y envía la mercadería, y confirma el envío.
8. Depósito registra la recepción, actualiza y verifica el stock físico, y deja la reposición disponible para las
ventas siguientes

# Compuertas lógicas y excepciones:
Compuerta:                  Decisión:                                 Camino normal:               Excepción:
Gateway exclusiva XOR       Hay stock disponible?                     Sí: se registra la venta     No: se informa falta de stock y se genera pedido de reposición.
Gateway exclusiva XOR       El stock quedó por debajo del mínimo?     No: se mantiene la venta     Si: se genera alerta y pedido al proveedor.

# Diagrama actualizado: 
Diagrama_BPMN_corregido.png

# 4. Conclusion.

Esta entrega integra el análisis organizacional realizado en las instancias previas con herramientas de modelado, colaboración y gestión ágil. 
El diagrama BPMN permite comprender cómo el sistema de TecnoFácil S.R.L. automatizará el proceso de venta, control de stock y generación de información.
El uso de GitHub permite documentar el proyecto, controlar las versiones y evidenciar el trabajo colaborativo mediante ramas, commits y Pull Requests. 
Por su parte, el tablero ágil facilita el seguimiento de las historias de usuario y de sus estados.
Finalmente, los indicadores de control permiten auditar el desempeño del sistema y verificar si este contribuye a reducir errores, mejorar la trazabilidad, 
evitar faltantes de stock y facilitar la toma de decisiones.
