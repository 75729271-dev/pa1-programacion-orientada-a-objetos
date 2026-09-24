# Sustentación del proyecto

El PA1 desarrolla una aplicación Java por consola para registrar productos y controlar las existencias de una microempresa.

- [Video de exposición](https://www.youtube.com/watch?v=TKgLy1HdxAg).
- [Documento de sustentación en PDF](../output/pdf/Sustentacion_PA1.pdf).
- [Presentación PowerPoint](../output/presentations/Presentacion_PA1.pptx).

## Fundamentos de la solución

La clase Producto representa un artículo mediante su código, nombre, precio, stock y stock mínimo. Su constructor parametrizado inicializa esos datos. Los atributos privados permiten controlar los cambios mediante métodos: ingresarStock y retirarStock validan las cantidades antes de modificar las existencias.

Inventario reúne hasta cien productos, evita códigos duplicados y calcula las unidades y el valor total. Aplicacion contiene main y coordina la lectura de datos y las opciones del menú. La separación permite comprobar las reglas de los productos de manera independiente de la interacción por consola.

## Estructuras de control

| Estructura | Aplicación |
| --- | --- |
| if e if-else | Validar cantidades, disponibilidad y estados del stock |
| switch | Seleccionar la operación del menú |
| do while | Repetir el flujo principal hasta salir |
| while | Volver a solicitar entradas inválidas |
| for | Recorrer las posiciones ocupadas del inventario |
| Contadores | Registrar cantidad de productos y alertas |
| Acumuladores | Sumar unidades y valor de las existencias |

## Demostración

1. Registrar A01, Arroz, precio S/ 4.50, stock 10 y mínimo 3.
2. Registrar B01, Aceite, precio S/ 8.00, stock 2 y mínimo 2.
3. Intentar registrar A01 nuevamente: el código duplicado se rechaza.
4. Retirar 7 unidades de Arroz: quedan 3 y se activa la alerta de stock bajo.
5. Intentar retirar otras 4 unidades: el retiro se rechaza y el stock permanece en 3.
6. Ingresar 2 unidades de Arroz: el stock aumenta a 5.
7. Consultar el resumen: 2 productos, 7 unidades, 1 alerta y valor total S/ 38.50.

La valorización final es 5 × S/ 4.50 + 2 × S/ 8.00 = S/ 38.50. El retiro rechazado no altera las existencias.

## Verificación y alcance

Las pruebas registran 142 verificaciones de lógica y 14 escenarios de consola correctos. Incluyen duplicados, capacidad, cantidades inválidas, falta de stock, acumuladores y finalización de la entrada. Los detalles se encuentran en [pruebas.md](pruebas.md).

Los datos permanecen en memoria durante la sesión. El inventario admite 100 productos y los precios se representan con double, con redondeo y presentación a dos decimales. El alcance corresponde al uso de clases, atributos, constructores, métodos y estructuras de control de las sesiones 1 a 4.
