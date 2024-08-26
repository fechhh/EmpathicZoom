# EmpathicZoom

## Grupo 1
* Grijalba, Federico
* Richard, Federico
* Ruiz, Lautaro
* Szekieta, Paola

## Objetivo
Desarrollar una aplicación que permita reconocer las emociones de los participantes en una reunión de ZOOM.

## Dependencias/Librerias necesarias (como instalar ambiente)
Para realizar la ejecución de las notebooks es necesario realizar la intalacion de las dependencias del proyecto.

Las mismas se encentran en el archivo [requirements.txt](./requirements.txt).

Para su instalación mediante pip, se debe ejecutar desde la terminal:
```sh
pip install -r /path/to/requirements.txt
```

Recordar tener activado el ambiente del proyecto. El mismo puede ser definido con virtualenv.

Si se tiene instalado conda, se puede crear el ambiente mediante el archivo [environment.yml](./environment.yml). Para esto ejecutar desde la terminal:
```sh
conda env create -f environment.yml
```

## Uso del aplicativo

Este se desarrolla en la notebook `Main.ipynb`. 

Esta incluye las siguientes secciones:

1. Importar Librerías.
2. Definir rutas.
3. Definir funciones para la ejecución del aplicativo.
    
    Para entrar en una reunión de zoom YA INICIADA por otro usuario.
    
    Es necesario en esta parte de la notebook especificar:
    * MEETING ID (ej. 8015373437)
    * ACCESS CODE (ej. "8513")
4. **Ejecutar aplicación**.
    
    Ejecutar esta celda de código para ingresar a la reunión automáticamente con Selenium.
    
    Cada 10 segundos irá sacando un screenshot de la reunión e identificará las emociones de los usuarios hasta completar una máxima cantidad de screenshots definidos en el objeto 'screenshot_nro_max' (por default, son 3).
5. Propuestas de mejoras.