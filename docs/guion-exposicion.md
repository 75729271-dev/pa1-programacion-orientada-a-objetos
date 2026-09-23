# Guion propuesto de exposición

Duración orientativa: 6 a 8 minutos. Ajustar a las instrucciones del docente. Cada integrante participa con la cámara encendida. Este archivo prepara la grabación; no sustituye el video requerido.

## Integrante 1: caso y modelo

Presentar la necesidad de la microempresa y las operaciones del menú. Abrir `Producto.java` y explicar la diferencia entre una clase y un objeto. Mostrar los atributos de instancia, una constante de clase y el constructor parametrizado. Explicar por qué el stock se modifica mediante métodos.

## Integrante 2: inventario y cálculos

Mostrar el arreglo de productos y el contador `cantidad`. Explicar cómo se evita duplicar un código y cómo `for` visita solo las posiciones ocupadas. Distinguir el contador de productos del acumulador de unidades y del acumulador de valor monetario. Mencionar la capacidad fija y el almacenamiento temporal.

## Integrante 3: demostración del programa

1. Ejecutar la aplicación y listar el inventario vacío.
2. Registrar A01, Arroz, S/ 4.50, stock 10, mínimo 3.
3. Registrar B01, Aceite, S/ 8.00, stock 2, mínimo 2.
4. Intentar registrar A01 otra vez y explicar el rechazo.
5. Retirar 7 unidades de A01. Consultar su estado de stock bajo.
6. Intentar retirar 4 unidades de A01. Mostrar que el stock sigue en 3.
7. Ingresar 2 unidades de A01 y abrir el resumen: 2 productos, 7 unidades, 1 alerta, S/ 38.50.
8. Introducir una opción con letras y comprobar que el menú permite corregirla.

Relacionar `switch`, `do while`, `while` e `if` con lo observado.

## Integrante 4: pruebas y justificación

Ejecutar `PruebasInventario` y explicar al menos dos pruebas, incluidos un rechazo sin cambios y un cálculo del resumen. Mostrar la documentación del repositorio y comentar sus límites: memoria temporal, capacidad fija y uso educativo de `double`. Explicar qué mejoraría en una evaluación futura si se permitieran persistencia o colecciones.

## Preguntas para preparar la sustentación

- ¿Por qué stock mínimo y stock actual son atributos distintos?
- ¿Qué diferencia hay entre `mostrarInformacion` y `calcularValorStock`?
- ¿Por qué una cantidad negativa no debe modificar existencias?
- ¿En qué se diferencia `cantidad++` de `total += valor`?
- ¿Por qué un stock igual al mínimo activa una alerta?
- ¿Qué ocurre al cerrar el programa y por qué se eligió ese alcance?

Al finalizar, publicar la grabación en YouTube con la visibilidad indicada por el docente y colocar el enlace en el README. Revisar que el docente pueda abrir tanto el video como el repositorio.
