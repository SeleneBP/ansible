# Configurar un playbook en Ansible

Vamos a configurar nuestro primer script en ***Ansible***.

Antes de nada, un ***playbook***, nos permite gestionar la configuración del despliegue de aplicaciones en los nodos remotos. En los ***playbook*** describimos las configuraciones, las aplicaciones que queremos instalar, los pasos a seguir, etc. Esto se escribe en ficheros *yaml*.

(IMPORTANTE: En los ficheros *yaml*, NO se permiten tabulaciones, para indexar se utilizan espacios)

_______________________________________________________________________________________

Empezamos creando un directorio donde almacenaremos todos los archivos que crearemos del ***playbook***.

![image](https://user-images.githubusercontent.com/91204696/213911428-f5227f41-7b3f-4b14-bee7-4682017ce869.png)

El primer fichero que meteremos, es el fichero ***hosts***, que es para indicar los nodos sobre los cuales realizaremos los despliegues. 
En este caso solo tenemos un nodo, así que solo definiremos ese nodo.

Para definirlo ponemos entre corchete el grupo que va a identificar el nodo y la IP o el DNS de la máquina nodo.

![image](https://user-images.githubusercontent.com/91204696/213912167-5a43cdb7-97b5-4f3b-b4a6-797f30bff73b.png)

Ahora, generamos unas claves SSH para poder acceder al servidor remoto sin que solicite una clave.

![image](https://user-images.githubusercontent.com/91204696/213912239-5ed46696-798d-4e77-badf-d20dfe2c9170.png)

Copiaremos nuestra clave pública a la máquina nodo.

![image](https://user-images.githubusercontent.com/91204696/213912517-bf294abd-2b30-4bc1-a826-5ff22bd47e80.png)

Vamos a comprobar que podemos acceder al nodo, sin que nos pida la contraseña.

![image](https://user-images.githubusercontent.com/91204696/213912574-6a225cfd-ee2e-43ec-8c93-74eb4d02bbbd.png)

Ya podemos acceder sin clave, así que ya podemos configurar nuestro ***playbook***.
_________________________________________________________________________________________

Creamos un fichero *yaml*, dentro del directorio que hemos creado para el ***playbook***. Aquí meteremos el host sobre el que queremos desplegar el ***playbook*** y el usuario que queremos que utilice, también configuramos los *task*, que son las tareas, comandos o módulos que se ejecutan dentro del ***playbook***, siempre se ejecutan en orden, si alguno de los nodos falla, el nodo se eliminaría. Esto solo se ejecutaría si tuviese algo que hacer.

![image](https://user-images.githubusercontent.com/91204696/213913568-4d585726-a534-40d6-92f3-dbca328d2528.png)

