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







