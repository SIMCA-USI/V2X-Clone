# V2X-Clone
Script para instalar y clonar los módulos.
Imagen de referencia a usar: https://drive.upm.es/index.php/s/DuZ3ebIf09Qk4ms

# Uso
El script tiene que ser ejecutado como superusuario

```console
$ sudo python3 script.py -i {IMAGEN} -o {COMPACT FLASH} -id {ID DEL MÓDULO}
```

Ejemplo:
```console
$ sudo python3 script.py -i base_module.iso -o /dev/sdd -id 2
```

# Configuración
Hostname: V2X-{ID}

## WIFI
Para acceder por wifi, la IP es 192.168.1.1

SSID: V2X-{ID} Ejemplo: V2X-11, V2X-2

PWD: V2X_stati0n

## Cable
La subred es 192.168.0.X

Sin DHCP por defecto tras la instalación

Arranca con IP estática en la red 192.168.0.0/24, donde el número de terminal es el ID del módulo. Si el ID es 1, la IP tendrá como último octeto 254

Ejemplo: 192.168.0.11 para V2X-11, 192.168.0.2 para V2X-2, 192.168.0.254 para V2X-1

# Login
root:debian para módulos de despacho. Por determinar para módulos de carretera
