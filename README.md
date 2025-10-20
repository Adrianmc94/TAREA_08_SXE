# TAREA_08_SXE
## Instalacion de los servicios wiki, postgres y pgadmin
### Vamos a crear un directorio expresamente para esta práctica ya que es un buen repaso para el examen.
```bash
mkdir Sminulacro SXE 1er examen
```
### dentro del directorio creamos el archivo de configuración de servicios .yml
## Configuración de la DB Postgres y Wiki:

<img width="530" height="738" alt="image" src="https://github.com/user-attachments/assets/d8471d8f-8078-4f0f-aa23-13c6a100252a" />

esta configuracion la encontramos muy facil en el manual de la imagen Wiki

## Configuracion de pgadmin y volumenes:

<img width="528" height="441" alt="image" src="https://github.com/user-attachments/assets/f870854d-a528-4368-9ed8-5e12b2d7d34e" />

esta conf tambien la encontramos en el enlace de la imagen, pero no tan facil de completar....

### Corremos la nueva configuracion en docker
```bash
docker compose up
```
ATENCION!!
Hay q ver primero si algun de los otros servicios esta corriendo con el mismo puerto de escucha activado, en mi caso me paso con el 8080 de Wiki que estaba ya cogido por el de pretashop sin darme cuenta y no sabia pq me daba error de conexion, simplemente de damos stop al servicio y ya.

## Accedemos a pgadmin:
en nuestro navegador ponemos http://localhost:8081
<img width="947" height="902" alt="image" src="https://github.com/user-attachments/assets/a235ab48-e027-438e-b519-ef2a079c8107" />
Ponemos nuestras credenciales establecidas en el archivo .yml y podremos acceder:
<img width="1918" height="965" alt="image" src="https://github.com/user-attachments/assets/41647b2c-6208-484e-ad30-5144d09d21bd" />


## Accedemos a Wiki:
en nuestro navegador ponemos http://localhost:8080
<img width="1890" height="960" alt="image" src="https://github.com/user-attachments/assets/a415214f-4655-4ccc-9d35-5e3bf31eb0dc" />

<img width="1918" height="855" alt="image" src="https://github.com/user-attachments/assets/e2ee9fbd-62a7-4a4e-94ca-c8230c2f66ee" />

<img width="1917" height="977" alt="image" src="https://github.com/user-attachments/assets/8cb6f36b-f364-4551-a5b7-194556d31637" />
Aqui ya podemos ver como funciona, en este caso creé para ver como iba un proyecyo de HTML.

<img width="1918" height="962" alt="image" src="https://github.com/user-attachments/assets/bab2bc03-d8ed-4c64-b063-7e1b9d801556" />
Y alguna foto mas de la inferfaz de Wiki.













