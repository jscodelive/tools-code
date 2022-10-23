# Desinstalar git
Para eliminar solo el paquete git de Ubuntu, ejecute en la terminal:
```
$ sudo apt-get remove git
```
### Desinstalar git y sus paquetes dependientes
Para eliminar el paquete git y cualquier otro paquete dependiente que ya no se necesite de Ubuntu Trusty.
```
$ sudo apt-get remove --auto-remove git
```
### Purgando git
Si también desea eliminar los archivos de configuración y/o datos de git de Ubuntu Trusty, esto funcionará:
```
$ sudo apt-get purge git
```
Para eliminar los archivos de configuración y/o datos de git y sus dependencias de Ubuntu Trusty, ejecute:
```
$ sudo apt-get purge --auto-remove git
