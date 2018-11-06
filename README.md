# hack_iia
Introducción a la Inteligencia Artificial - Curso Hack Academy

# Configuracion de entorno

## Linux/MacOS

Primero instalar python3.6 y git:

En Ubuntu (Linux):
```
$ sudo apt-get install python3-pip python3-dev git
```

Desde la Maquina Virtual distribuida con Ubuntu (Linux) sólo este comando:
```
$ sudo apt install python3-pip git
```

En OSX debemos primero instalar Homebrew y git:
```
$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
$ brew install git
```

Luego correr el siguiente comando en consola:
```
$ brew install https://raw.githubusercontent.com/Homebrew/homebrew-core/f2a764ef944b1080be64bd88dca9a1d80130c558/Formula/python.rb
```

Una vez instalado Python se debe continuar de la siguiente manera. Primero crear una carpeta por ejemplo "cursoai"
Luego desde esa carpeta descargar el repositorio utilizando el siguiente comando:
```
$ git clone https://github.com/MatiTaila/hack_iia.git

```

Luego desde consola instalar "virtualenv" y crear un virtual environment con nombre "ha_env"

```
$ sudo pip3 install virtualenv
$ virtualenv -p python3 ha_env
```
Una vez creado se debe activar de la siguiente manera::

```
$ source ha_env/bin/activate
```

Se prosigue a instalar las dependencias:
```
$ pip3 install -r requirements.txt
```
Luego simplemente desde consola moverse al directorio "hack_iia" y levantar el entorno de desarrollo:
```
$ cd hack_iia
$ jupyter notebook
```

No olvidarse al terminar de trabajar ejecutar:
```
deactivate
```

## Windows

En Windows debemos primero instalar Anaconda:

```
Descargar Anaconda: https://repo.anaconda.com/archive/Anaconda3-5.2.0-Windows-x86_64.exe
```

Virtualenv
```
Se crea con el siguiente comando:
conda create --name env python=3.5
```
Activamos el entorno virtual: 
```
activate env
```

Actualizamos el gestor de paquetes:
```
python -m pip install --upgrade pip
```

Descargamos el repositorio:
```
git clone http://www.github.com/MatiTaila/hack_iia.git
```
Para completar la instalación de los paquetes requeridos debemos navegar hasta el directorio del repositorio y luego ejecutar:
```
pip install -r requirements.txt
```
Luego navegar hasta el directorio "hack_iia" y levantar el entorno de desarrollo con el siguiente comando:
```
jupyter notebook
```

