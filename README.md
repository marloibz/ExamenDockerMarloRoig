# ExamenDockerMarloRoig

## Apartado 1 
### Ejericio 1
1. Descargamos la imagen que nos piden es esta caso ubuntu:18.04
![Captura](https://user-images.githubusercontent.com/91874499/173302394-5c26c435-3315-4926-ae1d-0cbb868c52ef.PNG)
2. Realizamos un docker images para ver que se haya descargado la imagen correctamente 
![Captura](https://user-images.githubusercontent.com/91874499/173302554-63dd0c3d-45cd-42ea-b99d-c1b002a18240.PNG)
3. Ejecutamos el contener 
![Captura](https://user-images.githubusercontent.com/91874499/173302914-d72f42e8-e9d6-42c5-8273-2338d74238a3.PNG)
4. Realizamos un :ls para ver donde estamos y haremos un :cd para ir a var

Así es como queda la consola al finalizar la tarea
![Captura](https://user-images.githubusercontent.com/91874499/173303308-d503d9b6-7273-4285-8efc-4e34cd730ae2.PNG)


### Ejericio 2
1. Realizamos un docker ps -a para ver los contenedores que tenmos
![Captura](https://user-images.githubusercontent.com/91874499/173303736-342897eb-1b4c-41e7-8b18-78e6ecd9eea3.PNG)
2. Descargamos la imagen centOS:latest
![Captura](https://user-images.githubusercontent.com/91874499/173304633-b6f761e5-6187-462f-8567-dbd892a40208.PNG)
3. Miramos las imagenes que tenemos
![Captura](https://user-images.githubusercontent.com/91874499/173304918-826d3ac8-fcfb-40ae-9009-1bd65543130b.PNG)
4. Ejecutamos el comando de indicado y además nos debe mostrar los directorios que hay porque añadimos al final :ls
![Captura](https://user-images.githubusercontent.com/91874499/173304976-a9d4f71c-29d0-4163-a900-cbc605e8ed50.PNG)

### Ejercicio 3
1. Ejecutamos el comando que indican y nos muestra lo siguiente:
![Captura](https://user-images.githubusercontent.com/91874499/173305387-6f9d5a7a-ceb3-4ea9-85d4-f073663bf197.PNG)

Vemos que se crea un servidor Web Apache 2.4 en la ip mostrad:127.17.0.2

### Ejercicio 4
1. Ejecutamos el comando :docker run -it -w /etc debian:9 ls , como no tenemos la imagen con la misma instrucción se descargará la imagen
Para que muestre el contenido de una carpeta establecida con el parámetro -w , yo he puesto /etc
![Captura](https://user-images.githubusercontent.com/91874499/173306264-f5c45dbe-a2ee-44c9-9b62-6a8ae600a439.PNG)


Al finalizar los ejericios del apartado 1 realizo los comandos :
- Docker ps (muetra los contenedores activos) que no hay ninguno 
- Dcoker ps -a (muestra todos los contenedores que hayamos usado) hay unos cuantos junto con unas pruebas realizadas
- Docker images (muestras las imagenes descargadas) hay 4

![Captura](https://user-images.githubusercontent.com/91874499/173307291-445ea61b-14cd-4440-b84f-093fd126e9be.PNG)


## Apartado 2

### Dockerfile Tomcat
1. Empezamos creando un reposidotrio para guardar el DockerFile que lo llamaré repoExamen
2. Miro que se haya creado y me dirijo a él
![Captura](https://user-images.githubusercontent.com/91874499/173307707-fad09e7d-4b98-4ac6-b01b-fa99a1b2617a.PNG)
3. Ahora creo y compruebo que esta creado el archivo Dockerfile

![Captura](https://user-images.githubusercontent.com/91874499/173307951-82ac7681-18b8-474d-ac78-941a5cca42d8.PNG)
4. Con la instrucción : vi Dockerfile editamso el archivo (no he podido hacer de tomcat porque la maquina se me paraba todo el rato y no me dejaba hacer el build):
- La imagen de origen que será :debian:latest
![Captura](https://user-images.githubusercontent.com/91874499/173312468-895891e7-5f98-42a0-a040-9ee6eabcb24d.PNG)
5.Ahora creamos la imagen y le ponemos de nombre: debian-m

![Captura](https://user-images.githubusercontent.com/91874499/173312841-fa9462b0-ff36-477f-810b-089dd5e47a19.PNG)
6. Nos logeamos para poder hacer el push
![Captura](https://user-images.githubusercontent.com/91874499/173313057-7b01c89b-cda9-4c30-9b9a-7489ff885d25.PNG)
7. Ponemos a la imagen el nombre de usuario nuestro y comprobamos que se ha generado correctamente
![Captura](https://user-images.githubusercontent.com/91874499/173313485-df8f2fab-5092-415d-afda-86feeaaf3ecf.PNG)
8. Subimos la imagen generada a nuestro dockerhub
![Captura](https://user-images.githubusercontent.com/91874499/173313744-6f66225e-88eb-48d8-8158-728bd5eae5c6.PNG)
9. Comprobamos que se ha subido al docker hub
![Captura](https://user-images.githubusercontent.com/91874499/173313884-3a51714c-24c5-4bc5-84f0-0bd3451e9348.PNG)

10. Aquí el link de la imagen subida a mi dockerHub
https://hub.docker.com/r/vaquer/debian-m 




