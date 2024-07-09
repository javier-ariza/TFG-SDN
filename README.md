# TFG-SDN
Archivos utilizados para el TFG "Desarrollo y evaluación de una red definida por software con conmutadores físicos" ETSIT-UPM (2024)

A continuación, se detalla por bloques cada uno de los archivos existentes en este repositorio.


Bloque I: Carpeta de archivos de configuración de escenarios virtualizados VNX. Se han desarrollado a partir de los ejemplos de [1] Se selecciona el escenario en función del número de conmutadores (1 o 3) y el controlador SDN (Ryu u ONOS). Por ejemplo: Para un conmutador con el controlador SDN Ryu se despliega el escenario 1-SW-RYU. Se utiliza con VNX previamente instalado, y despliega el escenario con el comando:

sudo vnx -f 1-SW-RYU.xml -t


Bloque II: En el archivo 'ConfiruacionDeConmutadores' se encuentra la configuración de los conmutadores SDN cuando se desplegó la topología de red con tres conmutadores gobernados por el mismo controlador SDN. Los comandos utilizados en estas configuraciones (y el resto en el desarrollo del TFG) se encuentran en la guía openflow de los conmutadores Dell [2] y Aruba [3]

Bloque III: Por último, en este repositorio se encuentra la aplicación para el controlador Ryu denominada simple_switch_13_tagged.py. Este aplicación se ha desarrollado a partir de [4]. Para lanzarla se ejecuta el siguiente comando desde un terminal en el controlador c0:

ryu-manager ryu.app.simple_switch_13_tagged


Referencias:

[1] DIT, «Virtual Networks over linuX (VNX),» [En línea]. Available:  https://web.dit.upm.es/vnxwiki/index.php/Main_Page. [Último acceso: Mayo 2024].

[2] Dell, Inc., «Dell OpenFlow Deployment and User Guide 4.0,» 2017. [En línea]. Available: https://dl.dell.com/manuals/all-products/esuprt_ser_stor_net/esuprt_networking/esuprt_net_netwrkng_sw/force10-sw-defined-ntw_deployment%20guide4_en-us.pdf [Último acceso: Junio 2024].

[3] Hewlett Packard Enterprise Development LP., «Aruba OpenFlow 1.3 Administrator Guide for  ArubaOS-Switch 16.07,» 2018. [En línea]. Available: https://techhub.hpe.com/eginfolib/Aruba/16.07/5200-5374/index.html#c_Configuring_OpenFlow.html. [Último acceso: Junio 2024].

[4] Departamento en Ingeniería de Sistemas Telemáticos, «Prácticas 2.4 y 2.2 de la asignatura RDSV/SDNV del MUIT de la ETSIT (UPM),» DIT, Madrid, 2024

