# Inventario.
# Sistema de Inventario Simple

Este proyecto es un programa en Python que permite gestionar de manera básica un inventario de productos. El usuario ingresa el nombre, el precio y la cantidad de un producto, y el programa calcula automáticamente el costo total.

## Funcionalidades

1. Solicitar el nombre del producto:
   - El nombre **no puede estar vacío**.
   - Debe contener **solo letras**.

2. Solicitar el precio del producto:
   - Debe ser un **número válido**.
   - No puede ser negativo.

3. Solicitar la cantidad del producto:
   - Debe ser un **número entero válido**.
   - No puede ser negativo.



4. Calcular el costo total:
   ```python
   costo_total = precio * cantidad
   
   
5. Mostrar un resumen en pantalla
 -  Producto: <nombre> | Precio: <precio> | Cantidad: <cantidad> | Total: <costo_total>
 - === SISTEMA DE INVENTARIO ===
 - Ingrese el nombre del producto: Manzana
 - Ingrese el precio del producto: 2.5
 - Ingrese la cantidad del producto: 10
 - === RESULTADO DEL INVENTARIO ===
 - 
Producto: Manzana | Precio: 2.5 | Cantidad: 10 | Total: 25.0



# Validaciones y errores manejados

Nombre vacío → mensaje de error.

Nombre con números o símbolos → mensaje de error.

Precio negativo o no numérico → mensaje de error.

Cantidad negativa o no entera → mensaje de error.

# Cómo ejecutar

1.Clonar o descargar el repositorio.

2.Ejecutar el archivo inventario.py con Python 3

   


