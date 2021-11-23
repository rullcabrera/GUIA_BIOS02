author: Raúl Cabrera Garcia
summary: Guia Opciones Seguridad BIOS2
id: BIOS02
categories: codelab,markdown
environments: Web
status: Published
feedback link: [Enlace para dejar un issue en Git Hub](https://github.com/rullcabrera/GUIA_BIOS02/issues)

# GUÍA BIOS 02 ThinkPad E15 (20RD 20RE)

## Página 1
Duration 00:00:30

### Introducción

En este caso se trata de una *BIOS UEFI* también, pero mucho más actual.
Muestro en la siguiente página la lista de opciones de seguridad que tenemos disponibles.

![Foto1_BIOS02](img/foto_portatil2.jpg)

## Página 2
Duration 00:04:00

### SECCIÓN PRINCIPAL OPCIONES DE SEGURIDAD

![Foto1_BIOS02](img/foto15.jpg)

Positive
: Os muestro un listado de las secciones y las vamos explicando:

### SECCIÓN PASSWORD

![Foto1_BIOS02](img/foto16.jpg)

* **Supervisor Password**: → Habilitar/Deshabilitar. Para asignar una clave de Supervisor, que nos pedirán al entrar en la BIOS.

![Foto1_BIOS02](img/foto_16_1.jpg)

![Foto1_BIOS02](img/foto_16_2.jpg)

* **Lock UEFI BIOS Settings**: → Nos permite bloquear las opciones de la *BIOS*, para no poder modificar sin antes poner la clave de *Supervisor*.

![Foto1_BIOS02](img/foto_16_3.jpg)

* **Password at Unattended Boot**: → Pedir la clave a la hora de un arranque desatendido. Por ejemplo; al usar el arranque por *WOL (Wake On Lan)*. Podríamos deshabilitar como medida de seguridad externa. Ya que no se podría arrancar el equipo mediante Red.

![Foto1_BIOS02](img/foto_16_4.jpg)

* **Password at Restart**: → Nos pedirá una clave al reiniciar el equipo.

![Foto1_BIOS02](img/foto_16_5.jpg)

* **Password at Boot Device List**: → Clave para acceder a la lista de dispositivos de arranque.

![Foto1_BIOS02](img/foto_16_6.jpg)

* **Password Count Exceeded Error**: → Habilitar un contador de ingreso erróneo de clave, a la hora de entrar a la *BIOS*.

![Foto1_BIOS02](img/foto_16_7.jpg)

* **Set minimum length**: → Activar un mínimo de longitud a la clave.

![Foto1_BIOS02](img/foto_16_8.jpg)

* **Power-On-Password**: → Habilitar el pedir una clave al arrancar el equipo. Se debe activar **“Password Beep”**, en el submenú **“Alarm”**. Para poder habilitar esta opción. Tiene el mismo proceso que **“Supervisor Password”**.

![Foto1_BIOS02](img/foto_16_9.jpg)

* **Hard disk 1 Password**: → Habilitar una clave al primer disco duro. Esta opción también requiere previamente activar la característica de **“Password Beep”**.
* Tendremos 2 opciones:
    *    **User only**: Se usa la clave del usuario que hemos configurado.
    *    **User+Master**: En este caso la del usuario y opcionalmente una clave **“maestra”**, puede usar para dar acceso al *Administrador*.

![Foto1_BIOS02](img/foto_16_10.jpg)

![Foto1_BIOS02](img/foto_16_11.jpg)

## Página 3
Duration: 00:01:00

### SECCIÓN SECURITY CHIP

Positive
: En esta sección podremos modificar opciones relativas al chip de seguridad *“TPM”*.

![Foto1_BIOS02](img/foto17.jpg)

* **Security Chip type**: → Vemos el tipo de chip de seguridad que tenemos instalado. En este caso *“TPM 2.0”*.
* **Security Chip**: → Podremos activar/desactivar el chip de seguridad.

![Foto1_BIOS02](img/foto_17_1.jpg)

* **Security Reporting Options**: → Tenemos un submenú con opciones de reporte de seguridad.
* **SMBIOS Reporting**: → Podremos habilitar/deshabilitar los reportes de información que produzca nuestra *BIOS*.

![Foto1_BIOS02](img/foto_17_2.jpg)

* **Clear Security Chip**: → Nos sirve para limpiar la claves de encriptación del Chip. No podremos acceder a la información encriptada que tuviéramos en el chip.

![Foto1_BIOS02](img/foto_17_3.jpg)

![Foto1_BIOS02](img/foto_17_4.jpg)

* **Physical Presence for Clear**: → Podremos habilitar/deshabilitar que nos salga una ventana para asegurar que un usuario físico debe de confirmar o no el limpiado del Chip.

![Foto1_BIOS02](img/foto_17_5.jpg)

## Página 4
Duration: 00:00:30

### SECCIÓN UEFI BIOS UPDATE OPTION

Positive
: Esta sección nos da opciones respecto a la actualización de la *BIOS*.

![Foto1_BIOS02](img/foto18.jpg)

* **Flash BIOS Updating by End-Users**: → Podremos poner si queremos que a la hora de actualizar nuestra *BIOS* requiera meter **“Supervisor Password”** o no.

![Foto1_BIOS02](img/foto_18_1.jpg)

* **Secure Rollback Prevention**: → Permite o no, el querer realizar *“flasheos”* a versiones de *UEFI BIOS* anteriores o no.

![Foto1_BIOS02](img/foto_18_2.jpg)

* **Windows UEFI Firmware Update**: → Nos permite activar/desactivar la opción de tener actualización de firmware *UEFI* de Windows.

![Foto1_BIOS02](img/foto_18_3.jpg)

## Página 5
Duration: 00:00:30

### SECCIÓN MEMORY PROTECTION

Positive
: En esta sección tenemos una opción respecto a protección de memoria de posibles *“virus”*.

![Foto1_BIOS02](img/foto19.jpg)

![Foto1_BIOS02](img/foto_19_1.jpg)

* **Execution Prevention**: → Podremos activar/desactivar siempre que nuestro sistema operativo lo permita. Esta opción puede prevenir de ataques *virus/gusanos* que se puedan crear a través de un **“Buffer Overflow”**. Si lo tenemos desactivado, estará el sistema en estado normal.

## Página 6
Duration: 00:00:30

### SECCIÓN VIRTUALIZACIÓN

Positive
: En esta sección tenemos opciones relativas a la virtualización. Para tener mejor compatibilidad luego con aplicaciones de máquinas virtuales. En este caso son tecnologías de *INTEL*.

![Foto1_BIOS02](img/foto20.jpg)

## Página 7
Duration: 00:01:00

### SECCIÓN I/O PORT ACCESS

Positive
: En esta sección hay opciones para decidir qué dispositivos de entrada/salida están activos.

![Foto1_BIOS02](img/foto21.jpg)

* **Ethernet LAN**: → Habilitar/Deshabilitar la tarjeta de red y en el sistema.
* **Wireless LAN**: → “”  “”  la tarjeta Wi-Fi.
* **Bluetooth**: → “”   “”  el chip bluetooth.
* **USB Port**: → “”    “” los puertos *USB*; no afecta a puerto **“Thunderbolt”** o puerto * **USB “Type-C”**.
* **Integrated Camera**: → “”    “” la cámara que nos viene con el portátil.
* **Microphone**: → “”    “” el micrófono que nos viene en el portátil.
* **Fingerprint Reader**: → “”  “” el lector de huellas del portátil.

## Página 8
Duration: 00:00:30

### SECCIÓN INTERNAL DEVICE ACCESS

Positive
: En esta sección tenemos una opción relativa al acceso de dispositivos internos; como el de almacenamiento.

![Foto1_BIOS02](img/foto22.jpg)

![Foto1_BIOS02](img/foto_22_1.jpg)

* **Internal Storage Temper Detection**: → Podremos activar/desactivar, activando nos detectará si hemos quitado algún dispositivo de almacenamiento interno o disco externo cuando el sistema está en modo hibernación. Si lo extraemos en ese estado el sistema se apagará y cuando vuelva arrancar desde la hibernación. Los datos no guardados se perderán.


## Página 9
Duration: 00:00:30

### SECCIÓN ABSOLUTE PERSISTENCIE(R) MODULE

Positive
: En esta sección podremos activar un módulo de persistencia. Es un servicio opcional de monitorización.

![Foto1_BIOS02](img/foto23.jpg)

* **Current Setting**: → Podremos habilitar/deshabilitar o permanentemente deshabilitado.
* **Current State**: → Se refleja la opción que elegimos arriba.

## Página 10
Duration: 00:01:00

### SECCIÓN INTEL(R) SGX CONTROL

Positive
: En esta sección tenemos opciones referidas al sistema de códigos de instrucciones relacionadas con la seguridad.

![Foto1_BIOS02](img/foto25.jpg)

* **Intel(R) SGX Control**: → Tenemos para habilitar/deshabilitar o que lo gestione el software *“SGX”* para *UEFI Boot OS*.
* **Current State**: → Refleja la opción elegida.

![Foto1_BIOS02](img/foto_25_1.jpg)

* **Change Owner EPOCH**: → Nos permite borrar la información persistente que tenga la tecnología de *INTEL SGX*.

![Foto1_BIOS02](img/foto_25_2.jpg)

## Página 11
Duration: 00:00:30

### SECCIÓN DEVICE GUARD

Positive
: En esta sección podemos decirle a la *BIOS* que deshabilite todas las opciones del **“Boot Order”**, y los deje solo a *HDD/SSD internos*.

![Foto1_BIOS02](img/foto26.jpg)

* **Device Guard**: → Podemos activar o no. Que solo se puede arrancar desde *HDD/SSD internos*. Para habilitar esta opción debe de estar activada **“Supervisor Password”**.

## Página 12
Duration: 00:00:30

### SECCIÓN THINKSHIELD SECURE WIPE

Positive
: En esta sección tenemos una opción para habilitar un **“Secure Wipe”**, a través de la *APP*.

![Foto1_BIOS02](img/foto27.jpg)

* **ThinkShield secure wipe in App Menu**: → Podemos activar/desactivar el *“ThinkShield Secure Wipe”* en el menú de la APP usando *F12*.

Negative
: Como hemos comentado arriba en distintos puntos, en esta *BIOS* tenemos varias opciones para evitar posibles arranques externos. Desde una amplia lista de dispositivos que podemos impedir que se puedan elegir como arranque. Que solo se puede arrancar el sistema desde discos duros internos. O también el impedir que se arranque con la opción **“Wake On Lan”**.

## Página 13
Duration: 00:02:00

### SECCIÓN SECURE BOOT CONFIGURATION

Positive
: **Secure Boot**: → En esta sección podremos configurar aspectos del **“Arranque Seguro”** que implementó *Microsoft*, para evitar en el arranque que pudieran cargar *drivers, firmware UEFI, OS etc..* de *“autores conocidos”*, evitando posibles archivos maliciosos.

![Foto1_BIOS02](img/foto24.jpg)

* **Secure Boot**: → Para activarlo o desactivarlo. Si lo activamos prevenimos que se arranquen por ejemplo *OS no autorizados*. Y tendremos que ponerlo en **“UEFI Only” and “CSM Support: no”**.

![Foto1_BIOS02](img/foto_24_1.jpg)

* **Platform Mode**: → Específicas el modo de proceder del sistema operativo. Tenemos 2 opciones **“User Mode” o “Setup Mode”**.
    * **User Mode**: El sistema mantiene la **“Platform Key”** para el **“Secure Boot”**.
    * **Setup Mode**: La **“Platform Key”** es limpiada en orden para personalizar las bases de datos del **“Secure Boot”** sin autorización.

![Foto1_BIOS02](img/foto_24_2.jpg)

* **Reset to Setup Mode**: → Esta opción sirve para resetear la actual **“Platform Key”** e instalar tu la tuya propia y personalizar las firmas de las bases de datos del arranque seguro.
* **Restore Factory Keys**: → Está opción sirve para restaurar de fábrica las claves y certificados de las base de datos del arranque seguro.
* **Clear All Secure Boot Keys**: → Nos permite limpiar todas las claves de las bases de datos que haya almacenadas en el arranque seguro. Y poder instalar tus propias claves y certificados.

## Página 14
Duration: 00:05:00

### SECCIÓN BOOT

Positive
: Boot, en esta sección vamos a poder configurar aspectos de cómo queremos que arranque el equipo, orden en el que queremos que lo haga o bloquear el poder modificar ese orden de arranque.

![Foto1_BIOS02](img/foto28.jpg)

* **Network Boot**: → Elegir el orden de prioridad en el arranque en Red cuando usemos **“Wake On Lan”**.

![Foto1_BIOS02](img/foto_28_1.jpg)

* **Boot Mode**: → Como queremos que sea el arranque, que nos muestre la pantalla de **“Diagnóstico”** o no.

![Foto1_BIOS02](img/foto_28_2.jpg)

* **Option Key Display**: → Que nos muestre o no las teclas de las opciones posibles en el arranque.

![Foto1_BIOS02](img/foto_28_3.jpg)

* **Boot Device List F12 Option**: → Habilitar/Deshabilitar que se nos muestre la opción de *F12* para lista los dispositivos de arranque. Solo podremos usar esta opción cuando el Supervisor entrar al *Setup*.

![Foto1_BIOS02](img/foto_28_4.jpg)

* **Boot Order Lock**: → Opción que nos permite bloquear para modificar el orden de arranque.

![Foto1_BIOS02](img/foto_28_5.jpg)