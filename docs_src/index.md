# Guía de Instalación y Configuración

![Python Logo](https://upload.wikimedia.org/wikipedia/commons/c/c3/Python-logo-notext.svg)

Bienvenido a esta guía rápida para instalar y configurar tu entorno de desarrollo en Python con PySide6.

---

## 🚀 Requisitos

✅ **Python 3.x**
✅ **pip (gestor de paquetes de Python)**

Si no los tienes instalados, sigue los pasos a continuación.

---

## 🔧 Instalación y Configuración

### 1️⃣ Instalación de Python 3 y pip

#### 🖥️ Windows
1. Descarga Python desde [python.org](https://www.python.org/downloads/).
2. Durante la instalación, marca la opción **"Add Python to PATH"**.
3. Verifica la instalación ejecutando en la terminal:

```sh
python --version
pip --version
```

#### 🐧 Linux
Para Debian/Ubuntu:
```sh
sudo apt update && sudo apt install python3 python3-pip -y
```
Para Fedora:
```sh
sudo dnf install python3 python3-pip -y
```
Verifica la instalación:
```sh
python3 --version
pip3 --version
```

---

### 2️⃣ Creación y Activación de un Entorno Virtual

Los entornos virtuales son esenciales para mantener tus proyectos organizados.

#### 🔹 Windows
```sh
python -m venv venv
venv\Scripts\activate
```

#### 🔹 Linux/Mac
```sh
python3 -m venv venv
source venv/bin/activate
```

Verás que el prompt de tu terminal cambia, indicando que el entorno virtual está activo.

---

### 3️⃣ Instalación de Dependencias

Con el entorno virtual activo, instala **PySide6** (para crear interfaces gráficas con Qt):
```sh
pip install PySide6
```

---

### 4️⃣ Creación de tu Primera Aplicación "Hola Mundo"

Ahora que todo está listo, crea un archivo `main.py` y agrega este código:

```python
from PySide6.QtWidgets import QApplication, QLabel
import sys

app = QApplication(sys.argv)
window = QLabel('🚀 ¡Hola, Mundo!')
window.show()
sys.exit(app.exec())
```

---

### 5️⃣ Ejecución de la Aplicación

📌 Para ejecutar el programa:

#### 🔹 Windows
```sh
python main.py
```

#### 🔹 Linux/Mac
```sh
python3 main.py
```