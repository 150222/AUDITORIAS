# Installed compiler(s)                                   [ ENCONTRADO ]

### Como solucionar el siguiente fallo con los siguientes comandos instalando es `ClamAV` con el comando.
```
sudo apt install clamav.
```
### Luego lo actualizas con el comando.
```
sudo freshclam
```
### Y después hacer un análisis del ordenador con 
```
sudo clamscan -r /home.
```
## Installed malware scanner                               [ NO ENCONTRADO ]

Lo primero seria ver si es necesario para ti, si no lo es no lo instales ya que puede crear otras brechas de seguridad.

## Non-native binary formats                               [ ENCONTRADO ]

Este mensaje indica que tienes compiladores instalados en tu sistema. Esto no es un fallo mas bien es un indicador no es necesario solucionar esto, pero si no necesitas un compilador en tu sistema por razones de seguridad (por ejemplo, para evitar que se compile código malicioso), puedes considerar eliminarlos.para eliminarlo seria con este

### Comando en linux:
 ```
 sudo apt remove gcc g++
```
```
sudo apt remove clang
```


## Installed malware scanner [NO ENCONTRADO]

Este mensaje indica que tu sistema no tiene instalado un escáner de malware. Esto es importante para proteger el sistema de virus, troyanos y otro software malicioso.

Solución: Debes instalar un programa de escaneo de malware dependiendo del sistema operativo que uses.

### Linux:
```
sudo apt update
```
```
sudo apt install clamav
```
### Luego, actualiza la base de datos de virus:
```
sudo freshclam
```
# Finalmente, puedes realizar un escaneo de todo tu sistema o una carpeta específica
```
sudo clamscan -r /home
```
## Non-native binary formats [ENCONTRADO]
Esto indica que en tu sistema están presentes formatos binarios que no son nativos del sistema operativo que estás utilizando, lo que podría implicar un riesgo de seguridad o simplemente estar usando herramientas como emuladores para ejecutar programas de otra plataforma.

### Solución Linux:
```
sudo apt remove wine
```
### También puedes buscar binarios no nativos utilizando el comando file para identificar los archivos:
```
file /ruta/al/binario
```
## Installed compiler(s) [ENCONTRADO]

### Este no es un error grave, simplemente te está informando que tienes compiladores instalados en tu sistema, lo cual es común en entornos de desarrollo o sistemas donde se necesita compilar código fuente.

### Solución Linux:

### Para eliminar compiladores como GCC o Clang, usa el siguiente comando
```
sudo apt remove gcc g++
```
```
sudo apt remove clang
```



