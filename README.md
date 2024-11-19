
# OpenStackServerUbutnto
Proyecto de openstack con ubuntto server

# instalacion del servicio openstack
```
sudo snap install microstack --beta >> para instalar los servicios de microstack
```
```
snap list microstack >> para ver la version de microstack 
```
```
sudo microstack init --auto --control >> iunicializa los servicio que necesita openstack  
```
# mostrar las maquinas virtuales 
```
microstack.openstack flavor list >> para ver las maquinas virtuales  con cada especificaciones de cada una
```
# crear maquina 
```
microstack launch cirros -n peri >> para poder crear la primera maquina virtual
```
# configurar el password para poder conectarnos al administrador web 
```
sudo snap get microstack config.credentials.keystone-password >> se crea una clave, con un usuario
    ---- https://localhost:443
```<< user: admin
   << costraseña:ul0HiSellKFiY481ZrvPDQVBFyNzJc8U
   << para poder ingresar a sitio web: 

# acceso de configuracion de openstack
  >> entramos para la consola en la cual ejecuta la maquina virtual dentro de la nube
  << la http://localhost:6082/spice_auto.html?token=13a9cf67-3c85-4f34-8353-b2b8dc65f1c2&title=peri(d0d42fc2-fc49-4945-9a28-d1fa6d8627e5)
``>> entramos por consola y nos da la misma consola un usuario y contraseña
  --- comando requridos:
  << pwd /// se entra a directorio de cirro
  << ls
  << cd /
  << ls
  <<
```
estos fueron los comandos requerido para poder implementar openstack con microstack


