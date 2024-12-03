# Ejercicio: Facturación de Múltiples Productos

Crea una página web que permita calcular el monto final a abonar para una lista de productos utilizando una función llamada `calcularFacturacion()`. Además, deberás mostrar un resumen detallado del total de productos procesados, los descuentos aplicados y el monto total a pagar utilizando **métodos de arrays** como `map`, `reduce` y `filter`.

---

## Requisitos

### 1. **Interfaz de usuario:**
- La página debe incluir:
  - Una tabla o lista donde el usuario pueda agregar múltiples productos con:
    - El nombre del producto.
    - El monto del producto.
    - El medio de pago (C: Crédito, E: Efectivo, D: Débito).
  - Un botón para **agregar** cada producto a la lista.
  - Un botón para **calcular el monto final** para todos los productos.
  - Un área para mostrar:
    - El detalle de cada producto con su descuento aplicado.
    - El total de productos procesados.
    - El monto total a abonar.

---

### 2. **Lógica de la función `calcularFacturacion()`:**
- **Entrada:** 
  Un array de objetos donde cada objeto representa un producto con las siguientes propiedades:
  - `nombre` (string): Nombre del producto.
  - `monto` (number): Precio del producto.
  - `pago` (string): Medio de pago (C, E, D).

- **Reglas de descuento:**
  - Si el monto del producto es menor a $200, no se aplicará ningún descuento.
  - Si el monto está entre $200 y $400:
    - Descuento del **30%** para pagos en efectivo.
    - Descuento del **20%** para pagos con tarjeta de débito.
    - Descuento del **10%** para pagos con tarjeta de crédito.
  - Para montos mayores a $400, se aplicará un descuento del **40%** sin importar el medio de pago.

- **Salida:**
  La función retornará un array con los productos actualizados, incluyendo:
  - El monto final de cada producto.
  - El descuento aplicado.

- **Resumen:** 
  Calcula y muestra:
  - El total de productos procesados utilizando `.length`.
  - El monto total acumulado utilizando `.reduce`.

---

### 3. **Métodos de Arrays:**
- **`map`:** Aplicar descuentos y calcular el monto final para cada producto.
- **`reduce`:** Calcular el total del monto a abonar.
- **`filter`:** Separar los productos que tienen un descuento aplicado (opcional).

---

## Ejemplo de Entrada y Salida

### **Entrada en la interfaz:**
| Producto       | Monto ($) | Medio de Pago |
|----------------|-----------|---------------|
| Televisor      | 500       | C             |
| Licuadora      | 350       | E             |
| Cafetera       | 150       | D             |

### **Salida esperada:**
- **Detalle de productos:**
  - **Televisor:** Monto original: $500, Descuento: 40%, Monto final: $300.
  - **Licuadora:** Monto original: $350, Descuento: 30%, Monto final: $245.
  - **Cafetera:** Monto original: $150, Descuento: 0%, Monto final: $150.
- **Total de productos procesados:** 3.
- **Monto total a abonar:** $695. 

---

## Entrega
1. El proyecto debe subirse a **GitHub** y publicarse en **GitHub Pages**.
2. La página debe tener estilos aplicados (CSS o Bootstrap).
3. Documenta en el repositorio:
   - El propósito del programa.
   - Capturas de pantalla mostrando su funcionamiento.
   - Pasos para utilizar la página.
