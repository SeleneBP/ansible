# Desplegar servicios en Ansible

Para desplegar el ***playbook*** de ***Ansible***:

`ansible-playbook -i hosts --ask-become-pass webserver.yml`

![image](https://user-images.githubusercontent.com/91204696/214068290-ca315832-96d0-4f8f-965e-991e36f545fc.png)

Ahora nos vamos a la máquina cliente y vemos que efectivamente se ha instalado *nginx*.

![image](https://user-images.githubusercontent.com/91204696/214074362-e2800d49-a4d0-4a8f-946b-7163acc09024.png)

Para hacer la comprobación, podemos hacerla a través del navegador, tanto de la máquina cliente como la del servidor, mientras se coloque la IP del cliente en la URL.

Vemos que se muestra correctamente el mensaje de bienvenida de *nginx*.

![image](https://user-images.githubusercontent.com/91204696/214075116-579dc68c-8ca5-4d01-81c0-c30cd6b85b93.png)

También podemos hacer la comprobación con el comando `curl IP`.

![image](https://user-images.githubusercontent.com/91204696/214075316-f01d70d4-fa17-44d9-be98-e9cebc829935.png)
