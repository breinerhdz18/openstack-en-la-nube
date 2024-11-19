
# OpenStackServerUbutnto
Proyecto de openstack con ubuntto server

# instalacion del servicio openstack
##  para instalar los servicios de microstack
```
sudo snap install microstack --beta 
```
##  para ver la version de microstack
```
snap list microstack  
```
##  inicializar los servicio que necesita openstack
```
sudo microstack init --auto --control   
```
# mostrar las maquinas virtuales 
```
microstack.openstack flavor list 
```
# crear la primera maquina virtual.
```
microstack launch cirros -n peri
```
# configurar el password para poder conectarnos al `administrador web` 
## se crea una clave, con un usuario
```
sudo snap get microstack config.credentials.keystone-password
```
## entrar en la configuracion web de openstack
```
https://localhost:443
```
## configuración para poder acceder a openstack
<< `user`: admin
<< `costraseña`:ul0HiSellKFiY481ZrvPDQVBFyNzJc8U
 

## acceso de configuracion de openstack
entramos para la consola en la cual ejecuta la maquina virtual dentro de la nube
```
http://localhost:6082/spice_auto.html?token=13a9cf67-3c85-4f34-8353-b2b8dc65f1c2&title=peri(d0d42fc2-fc49-4945-9a28-d1fa6d8627e5)
```
_NOTA_: Recuerde abrir los puerto en el virtualbox de los comandos que vaya abriendo por cada maquina virtual, por ejemplo el puerto del  comando anterior que es `6082`





