# 📦 Sistema de Inventario Básico en Python

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Estado](https://img.shields.io/badge/Estado-Educativo-green)
![Licencia](https://img.shields.io/badge/Licencia-MIT-orange)

---

# 📖 Descripción

Este proyecto consiste en un **sistema básico de inventario desarrollado en Python** que permite registrar información de un producto y calcular automáticamente su **costo total**.

El programa solicita al usuario los siguientes datos:

* Nombre del producto
* Cantidad de unidades
* Precio unitario

Posteriormente, el sistema valida los datos ingresados para evitar errores y muestra un **resumen del producto registrado** junto con el **total a pagar**.

Este proyecto está diseñado con fines **educativos**, ideal para personas que están comenzando a aprender **programación en Python**.

---

# 🎯 Objetivos del Proyecto

* Practicar conceptos básicos de programación en Python.
* Implementar validación de datos ingresados por el usuario.
* Comprender el uso de estructuras de control como **bucles (`while`)**.
* Aplicar manejo de errores con **`try` y `except`**.
* Desarrollar lógica básica de cálculo en programas interactivos.

---

# ⚙️ Características

✅ Validación de nombre de producto  
✅ Verificación de cantidad como número entero positivo  
✅ Validación de precio como número positivo  
✅ Manejo de errores en la entrada de datos  
✅ Cálculo automático del costo total  
✅ Resumen claro de la información ingresada  

---

# 🗂️ Estructura del Proyecto

inventario-python/

| Archivo       | Descripción                               |
| ------------- | ----------------------------------------- |
| inventario.py | Contiene el código principal del programa |
| README.md     | Documentación del proyecto                |

---

# 💻 Requisitos

Para ejecutar este programa necesitas:

* **Python 3.x**

Puedes descargarlo desde:  
https://www.python.org/downloads/

Para verificar que Python está instalado correctamente puedes usar:


```bash
python --version
```bash
python --version
```
---

### ▶️ Instalación y Ejecución

1️⃣ Clonar el repositorio

```bash
git clone https://github.com/tuusuario/inventario-python.git
```

2️⃣ Acceder a la carpeta del proyecto

```bash
cd inventario-python
```

3️⃣ Ejecutar el programa

```bash
python inventario.py
```
   
---
🖥️ Código del Programa
# Programa de inventario simple
# Solicita nombre, precio y cantidad de un producto
# Calcula el costo total y muestra los resultados

print("=== SISTEMA DE INVENTARIO ===")

# Solicitar nombre
while True:
    nombre = input("Ingrese el nombre del producto: ")
    if not nombre:
        print("Error: el nombre no puede estar vacío")
    elif not nombre.isalpha():
        print("Error: solo debe contener letras")
    else:
        break

# Solicitar precio
while True:
    try:
        precio = float(input("Ingrese el precio del producto: "))
        if precio < 0:
            print("Error: ingrese un valor correcto")
        else:
            break
    except ValueError:
        print("Error: debe ingresar un número válido para el precio")

# Solicitar cantidad
while True:
    try:
        cantidad = int(input("Ingrese la cantidad del producto: "))
        if cantidad < 0:
            print("Error: ingrese un valor correcto")
        else:
            break
    except ValueError:
        print("Error: debe ingresar un número entero válido para la cantidad")

# Calcular costo total
costo_total = precio * cantidad

# Mostrar resultado
print("\n=== RESULTADO DEL INVENTARIO ===")
print(f"Producto: {nombre} | Precio: {precio} | Cantidad: {cantidad} | Total: {costo_total}")








