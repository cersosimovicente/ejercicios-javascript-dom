# Página Web para Calcular el Monto Final a Abonar de un Producto

## Descripción

Crear una página que permita calcular el monto final a abonar de un producto, aplicando descuentos según el medio de pago y el monto ingresado. Utiliza la función `facturacion()` para procesar los cálculos basándose en las reglas de descuento definidas.

---

## Requisitos

### Interfaz de Usuario

La página debe incluir:

- Un **campo de entrada** para ingresar el monto del producto.
- Un **conjunto de botones** o un **menú desplegable** para seleccionar el medio de pago:
  - **C**: Tarjeta de Crédito
  - **E**: Efectivo
  - **D**: Tarjeta de Débito
- Un **botón** para calcular el monto final.
- Un **área** para mostrar el resultado del monto final a abonar.

---

### Lógica de la Función `facturacion()`

#### Parámetros:
1. **Monto del producto** ingresado por el usuario.
2. **Medio de pago** seleccionado.

#### Reglas de Descuento:
1. **Monto menor a $200:** No se aplica ningún descuento.
2. **Monto entre $200 y $400:**
   - 30% de descuento para pagos en efectivo.
   - 20% de descuento para pagos con tarjeta de débito.
   - 10% de descuento para pagos con tarjeta de crédito.
3. **Monto mayor a $400:** Se aplica un 40% de descuento sin importar el medio de pago.

#### Retorno:
La función devuelve el monto final calculado.

---

## Entrega

1. **Subir el proyecto** a un repositorio en GitHub.
2. **Publicar la página** en GitHub Pages.

---

## Documentación en el Repositorio

1. **Propósito del programa.**
2. **Instrucciones de uso.**
3. **Capturas de pantalla** de la página en funcionamiento.

---

## Notas Técnicas

- **Tecnologías utilizadas:** HTML, CSS, y JavaScript.
- **Validaciones:** Asegúrate de que los campos sean validados antes de realizar el cálculo (por ejemplo, verificar que el monto ingresado sea un número válido).
- **Estilos:** Aplica estilos básicos utilizando CSS o Bootstrap.

--- 
