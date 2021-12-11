# Dashboard con Jupyter Notebook, DASH, MongoDB y CoinGecko API

Este trabajo se realizo como parte de la maestría en ciencia de datos de la Universidad de Sonora

Se utilizo la api de CoinGecko para obtener la información de los precios de las criptomonedas:
Bitcoin
Ethereum
Shiba-Inu


## Requisitos previos  
- Docker
- Git
- Python

## Pasos para reproducir el trabajo realizado

1. Clonar el repositorio  
   ```git clone https://github.com/danielmc81/dashboard.git```
2. Iniciar MongoDB en un contenedor  
   ```sudo docker run -d -p 27017:27017 --network="host" --name=mongodb mongo```
3. Ejecutar MongoDB en terminal para crear nuestra base de datos  
   ```sudo docker exec -it mongodb bash```
5. Iniciar mongo.   
   ```mongo```
6. Crear la base de datos  
   ```use dasboard```
7. Lanzar la libreta con el dashboar desde la linea de comandos en otra terminal  
   ```jupyter nbconvert --execute dashboard.ipynb```
9. Abrir un explorador e ingresar la siguiente IP  
   ```http://127.0.0.1:8052/```
