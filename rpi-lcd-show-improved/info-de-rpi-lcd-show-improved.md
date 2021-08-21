---
description: 'Repo: https://github.com/PyPet/rpi-lcd-show-improved'
---

# Info de rpi-lcd-show-improved

## Cambios:

## Por Hacer:

* [ ] Desactivar el cambio de la configuración

## Instalar Drivers:

Los drivers de Balena no son perfectos con la pantalla de PyPetDIY, [Ver Problema](https://github.com/balenablocks/fbcp/issues/12).

Instalación con Balena

1. En "[fleets](https://dashboard.balena-cloud.com/fleets)" entra a tu fleet de PyPetDIY
2. Entra a "Devices"
3. Entra en tu dispositivo \(Normalmente es el único\)
4. En "Terminal", Accede como "Host OS" y Ejecuta el siguiente comando

{% hint style="warning" %}
NO uses otro usuario que no sea "Host OS"
{% endhint %}

```bash
curl -o- https://raw.githubusercontent.com/PyPet/rpi-lcd-show-improved/main/install | path_root=/ path_root_boot=/mnt/boot bash /dev/stdin tft35a
```

{% hint style="info" %}
Si se cambia alguna configuración del dispositivo, elimínala, PERO NO la del fleet \(el fleet tiene las configuraciones necesarias\)
{% endhint %}



