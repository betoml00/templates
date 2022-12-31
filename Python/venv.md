# Guía de entornos virtuales

## TL;DR
```
python -m venv ejemplo-env
ejemplo-env/Scripts/Activate.ps1
python -m pip install -r requirements.txt
```

## Creación de un entorno virtual

Para crear un entorno virtual, basta navegar a la carpeta en la que se creará el proyecto y luego correr la siguiente instrucción en una consola:
```bash
python -m venv ejemplo-env
```
En la carpeta del proyecto, se crea un nuevo directorio llamado `ejemplo-env`.

## Activación de un entorno virtual
En el directorio del proyecto, ejecutar uno de los siguientes comandos.
```bash
ejemplo-env/Scripts/activate.bat    // CMD
ejemplo-env/Scripts/Activate.ps1    // Powershell
```

## Uso de un entorno virtual
Una vez que el entorno virtual está activo, se puede hacer lo siguiente:

a. Instalar la versión más reciente de un paquete:
```bash
python -m pip install numpy
```
b. Instalar una versión específica:
```
python -m pip install numpy==1.24.1
```
c. Actualizar un paquete instalado:
```
python -m pip install --upgrade numpy
```
d. Exportar el entorno a un archivo `requirements.txt`:
```
python -m pip freeze > requirements.txt
```
e. Instalar los requerimientos de otro entorno:
```
python -m pip install -r requirements.txt
```

## Desactivar el entorno
Basta con correr el comando `deactivate`.

## Referencias
- [Documentación de Python](https://docs.python.org/3/tutorial/venv.html)
- [freeCodeCamp.org](https://www.freecodecamp.org/news/how-to-setup-virtual-environments-in-python/)