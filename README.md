# TFG-SDN
Archivos utilizados para el TFG "Desarrollo y evaluación de una red definida por software con conmutadores físicos" 
A continuación se detalla por bloques cada uno de los archivos existentes en este repositorio.

Bloque I: Carpeta de archivos de configuración de escenarios virtualizados VNX. Se han desarrollado a partir de los ejemplos de [1]
Se selecciona el escenario en función del numero de conmutadores (1 o 3) y el controlador SDN (Ryu u ONOS). Por ejemplo: Para un conmutador con el controlador
SDN Ryu se despliega el escenario 1-SW-RYU. Se utiliza VNX previamente instalado, y despliega el escenario con el comando:
vnx -t 1-SW-RYU.xml --create

Bloque II: 
