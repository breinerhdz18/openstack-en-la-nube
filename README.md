
# OpenStackServerUbutnto
Proyecto de openstack con ubuntto server

# instalacion del servicio openstack
```
 para instalar los servicios de microstack
sudo snap install microstack --beta 
```
```
snap list microstack >> para ver la version de microstack 
```
```
>> inicializar los servicio que necesita openstack
sudo microstack init --auto --control   
```
# mostrar las maquinas virtuales 
```
# para ver las maquinas virtuales  con cada especificaciones de cada una
microstack.openstack flavor list 
```
# crear maquina 
```
# para poder crear la primera maquina virtual
microstack launch cirros -n peri
```
# configurar el password para poder conectarnos al administrador web 
```
# se crea una clave, con un usuario
sudo snap get microstack config.credentials.keystone-password
  << https://localhost:443
   << user: admin
   << costraseña:ul0HiSellKFiY481ZrvPDQVBFyNzJc8U
   << para poder ingresar a sitio web: 

# acceso de configuracion de openstack
  #entramos para la consola en la cual ejecuta la maquina virtual dentro de la nube
  << la http://localhost:6082/spice_auto.html?token=13a9cf67-3c85-4f34-8353-b2b8dc65f1c2&title=peri(d0d42fc2-fc49-4945-9a28-d1fa6d8627e5)
# entramos por consola y nos da la misma consola un usuario y contraseña
  #comando requridos:
  << pwd /// se entra a directorio de cirro
  << ls
  << cd /
  << ls
  <<
```
estos fueron los comandos requerido para poder implementar openstack con microstack


