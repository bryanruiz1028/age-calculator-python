# 🐍 Python Precision Age Calculator (Calculador de Edad Exacta)

Un script de consola interactivo y de alta precisión lógica desarrollado en **Python 3**. Diseñado para calcular la edad exacta de una persona basándose en su fecha de nacimiento, integrando una validación estricta de días permitidos por mes y detección automatizada de años bisiestos.

[![Python](https://img.shields.io/badge/Python-3.x-blue?style=flat-square&logo=python)](https://www.python.org/)
[![CLI](https://img.shields.io/badge/Interface-CLI%20/%20Console-black?style=flat-square)](https://en.wikipedia.org/wiki/Command-line_interface)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?style=flat-square)](LICENSE)

---

## 🌟 Características Clave

*   **Detección de Años Bisiestos:** Lógica matemática automatizada para identificar si el año de nacimiento o el año actual son bisiestos, ajustando la duración de Febrero (28 o 29 días).
*   **Validación de Entradas Rigurosa:** Control de errores robusto que impide ingresar fechas imposibles (como el 30 de febrero o el 31 de abril), solicitando nuevamente el dato de forma interactiva.
*   **Mensaje Especial de Cumpleaños:** Si la fecha del cálculo coincide con el día y mes de nacimiento del usuario, el script despliega un mensaje dinámico de felicitación automatizado.
*   **Encapsulamiento en Funciones (`def`):** Modularización limpia y estructurada que facilita su integración directa en proyectos web más grandes (como Django o Flask).

---

## 🛠️ Detalle de Algoritmo y Funciones

*   **Detección bisiesta:** Implementa la regla astronómica gregoriana (divisible entre 4, no divisible entre 100 excepto si es divisible por 400).
*   **Control del calendario:** Mapeo de arreglos estáticos con límites de días por mes, adaptados dinámicamente según el año.
*   **Diferencia temporal:** Cálculo exacto de años, meses y días transcurridos desde el origen hasta el tiempo local (`datetime`).

---

## 🚀 Cómo Ejecutar en tu Computadora

Sigue estas instrucciones sencillas para descargar y correr el script en tu consola:

### 1. Clonar el Repositorio
```bash
git clone https://github.com/bryanruiz1028/age-calculator-python.git
cd age-calculator-python
```

### 2. Ejecutar el Script
Asegúrate de tener Python instalado y ejecuta el archivo:
```bash
python age_calculator.py
```

### 3. Interactuar con la Consola
El script te guiará solicitando:
*   El año de nacimiento (ej. `1995`)
*   El número de mes de nacimiento (ej. `2` para Febrero)
*   El día exacto de nacimiento. El script limitará dinámicamente tu input a los días que realmente existieron en ese mes de ese año particular.

---

## 📂 Estructura del Código

*   `age_calculator.py`: Contiene las funciones encapsuladas (`es_bisiesto`, `obtener_dias_mes`, `calcular_edad`) y el bucle principal de ejecución interactivo de consola.

---

## 📄 Licencia

Este proyecto está bajo la Licencia MIT - consulta el archivo [LICENSE](LICENSE) para más detalles.
