# V2X-Clone
Script para instalar y clonar los módulos.
Imagen de referencia a usar: https://drive.upm.es/index.php/f/168534976

# Uso
El script tiene que ser ejecutado como superusuario

```console
$ sudo python3 script.py -i {IMAGEN} -o {DISCO SD} -id {ID DEL MÓDULO}
```

Ejemplo:
```console
$ sudo python3 script.py -i base_module.iso -o /dev/sdd -id 2
```

# Configuración
Hostname: V2X-{ID}
## WIFI
SSID: V2X-{ID} Ejemplo: V2X-11, V2X-2
PWD: V2X_stati0n

## Cable
DHCP por defecto trás la instalación
IP estática en la red 192.168.0.0/24 donde el número de terminal es el ID del módulo.
Ejemplo: 192.168.0.11 para V2X-11, 192.168.0.2 para V2X-2 

# Login
root:debian