# Instalar Git para ubuntu 22.04!

Lo Primero que debemos realizar en abrir nuestra terminal podemos hacerlo con `Ctrl + alt + t`.


# Primer paso

Actualiza tu administrador de paquetes en  ubuntu con el comando

    sudo apt update

## Segundo Paso

Ahora solamente vamos a instalar desde nuestro administrador de paquetes el git usando el siguiente comando:

    sudo apt install git

Puedes revisar la revisión de Git usando:

    git --version

## Configuración Global de Git

Establezca su nombre de usuario y correo electrónico globales. Ejemplo:

    git config --global user.name "Jean Seijas"
    git config --global user.email "git@jscode.live"


## Confirmar configuración

Listado de las configuraciones globales de git se puede acceder con 

    git config --list


