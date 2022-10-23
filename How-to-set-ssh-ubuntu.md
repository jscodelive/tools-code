
## Pasos de configuración de la clave GitHub SSH

Para configurar las claves SSH de GitHub y usarlas en Ubuntu, siga estos pasos:

1. Cree un par de claves GitHub SSH con el [comando _ssh-keygen_]
2. Copie el valor de la clave SSH pública en el portapapeles
3. Inicie sesión en GitHub y navegue a la configuración de su cuenta
4. Haga clic en el enlace SSH y GPG
5. Haga clic en _Agregar clave_ para registrar la clave SSH pública con su cuenta
6. Asigne un nombre a la clave y pegue el valor copiado en el campo de texto
7. Guarda tus cambios
8. En su cliente Git, use la URL de GitHub basada en SSH para clonar su repositorio

Repasemos cada uno de estos pasos para configurar las llaves SSH de GitHub.

### Crear claves SSH de GitHub

En Ubuntu, las claves SSH que creas para GitHub deben ir en la carpeta _.ssh_. Realice toda la operación en esta carpeta:

    github@ubuntu:~$ cd ~/.ssh

Utilice el comando _ssh-keygen_ para crear pares de claves SSH de GitHub:

    github@ubuntu:~/.ssh$ ssh-keygen -o -t rsa -C "git@jscode.live"

La operación le pedirá que elija una ubicación en la que guardar las claves pública y privada. Simplemente haga clic en volver para dejarlos en la carpeta _.ssh_. El comando SSH se verá aquí cuando se realice un intento de conexión a un servidor remoto.


### Ubicación de la clave SSH de GitHub

Cuando se complete la operación de creación de la clave GitHub SSH, la terminal de Ubuntu mostrará una pieza muy satisfactoria de _randomart_.

También encontrará claves SSH públicas y privadas de GitHub en el directorio actual.

Deberá pegar el contenido de su clave SSH pública en GitHub. Cat el archivo para ver su contenido en la Terminal de Ubuntu y luego copiarlo:

    github@ubuntu:~/.ssh$ cat id_rsa.pub
