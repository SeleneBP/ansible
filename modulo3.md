# Instalación de Ansible

Lo primero que necesitaremos son dos máquinas virtuales. 
La primera es donde estará la instalación de ***Ansible***, tiene que tener salida a internet porque necesitaremos descargarnos el paquete.

![image](https://user-images.githubusercontent.com/91204696/213875018-18755b79-afe0-4317-9e20-93c50a9f8325.png)

La segunda máquina, es donde desplegaremos la aplicaciones de la máquina ***Ansible***.
(falta poner imagen ip)
_____________________________________________________________________________________________

En nuestra máquina principal, añadiremos los repositorios de ***Ansible***. 

`sudo add-apt-repository ppa:ansible/ansible`

![image](https://user-images.githubusercontent.com/91204696/213875265-81da6860-6a87-4bc1-92d1-4dde5c5ae61b.png)

Actualizaremos el sistema, para que los paquetes se actualicen.

![image](https://user-images.githubusercontent.com/91204696/213875383-d8e6e68d-b49d-4684-b72a-cd4e251fa0fa.png)

Por último, instalaremos ***Ansible*** y vemos su versión, para hacer una comprobación de que todo ha sido correcto.

![image](https://user-images.githubusercontent.com/91204696/213910678-9114ce51-10c4-489c-811b-176db84f4368.png)

![image](https://user-images.githubusercontent.com/91204696/213911157-bd60b81b-65c1-419a-b823-f9a7f9e4a404.png)
