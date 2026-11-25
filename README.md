# ChristopherJiemenez1020104396

Proyecto de la asignatura **Aplicaciones y servicios web** (ITM) que demuestra un flujo de **CI/CD con GitHub Actions**. El programa implementa operaciones aritméticas básicas en Python y cada cambio subido al repositorio ejecuta las pruebas automáticas.

![CI/CD Pipeline](https://github.com/Chrsitopherjim90/ChristopherJiemenez1020104396/actions/workflows/ci.yml/badge.svg)

## Descripción

El proyecto contiene:

- `sumar(a, b)`: devuelve la suma de dos números.
- `restar(a, b)`: devuelve la resta de dos números.
- Pruebas unitarias con **pytest** que verifican cada función.
- Un workflow de GitHub Actions que corre las pruebas en cada `push`.

## Estructura del proyecto

```
ChristopherJimenez1020104396/
├── .github/
│   └── workflows/
│       └── ci.yml        # Configuración del CI/CD
├── app.py                # Funciones del programa
├── test_app.py           # Pruebas automáticas
├── requirements.txt      # Dependencias
└── README.md             # Este archivo
```

## Requisitos

- Python 3.12 o superior
- Git

## Instalación y uso

1. Clonar el repositorio:

   ```bash
   git clone https://github.com/Chrsitopherjim90/ChristopherJimenez1020104396.git
   cd ChristopherJimenez1020104396
   ```

2. Instalar las dependencias:

   ```bash
   pip install -r requirements.txt
   ```

3. Ejecutar el programa:

   ```bash
   python app.py
   ```

4. Ejecutar las pruebas:

   ```bash
   pytest
   ```

## Flujo de CI/CD

El archivo `.github/workflows/ci.yml` se activa automáticamente con cada `push` a la rama `main`. El flujo realiza estos pasos:

1. Descarga el código del repositorio.
2. Configura Python 3.12.
3. Instala las dependencias de `requirements.txt`.
4. Ejecuta las pruebas con `pytest`.
5. Modificar las clases con suma y resta.

El resultado de cada ejecución se puede consultar en la pestaña "Actions" del repositorio.

## Autor

- Nombre: Christopher Jimenez Castillo
- Documento: 1020104396
- Programa: Desarrollo de software
- Institución: Institución Universitaria ITM
- Docente: Jonathan Sánchez Giraldo
