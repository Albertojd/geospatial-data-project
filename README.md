# geospatial-data-project

Comenzamos la busqueda de la nueva oficina en San Francisco.
En nuestra empresa somos 87 personas, dedicada al desarrollo de videojuegos, por lo que buscamos una oficina con los siguientes requisitos:

- Capacidad entre 90 y 120 personas
- Que se dedice al desarrollo de videojuegos, web, o software en general

Para ellos realizamos el siguiente filtrado en MongoDB compass:

```
{"offices.city":{$eq:"San Francisco"},
number_of_employees:{$gte:90, $lte:120},
"offices.latitude":{ $exists: true, $ne: null},category_code:{$eq:"games_video", $eq:"software", $eq:"web"}
```

![oficinas](images\oficinas.png)

A partir de aquí os mostraré como la ofcina de GitHub cumple con la mayoria de requesitos que plantea la empresa y por lo tanto, es la mejor candidata.
----------------------------------------------

A los diseñadores les gustaría tener cerca alguna startup que haya conseguido al menos $1M:
![alt text](images\millionoffice.png)

Vemos en el mapa, que en menos de 3km a la redonda tiene 4 startup que han conseguido 1 millón de dolares
############################################

Otra requisito indispensable es tener un aeropuerto cerca, y en este caso tenemos dos, el más cercano (San Francisco International Airport)a 17 kilomeros:
![alt text](images\airport.png)

## Los anteriores requesitos eran más imprescindibles a nivel empresarial, pero a continuación muestro el resto de servicios que demandan los trabajadores:

Tenemos un starbucks a 260 metros:
![alt text](images\coffe.png)

Aunque solo el CEO sea vegano, podriamos conciernos todos un poco y comer menos carne, en un area de 1km cuadrado encontramos 5 restaurantes veganos:
![alt text](images\vegan.png)


Para los trabajadores que tengan hijas e hijos, la zona cuenta con 6 colegios en 4 kilometros a la redonda:

![alt text](images\school.png)


Para después del trabajo tenemos tanto el estadio de los Golden State Warriors, a menos de 3 kilometros de la oficina, y una zona de pub nocutrnos a escasos metros de la oficna:
![alt text](images\afterwork.png)

Y por último, pero no menos importante, en menos de dos kilometros cuadrados hacía el sur, tenemos hata 5 peluquerias caninas para Pepe.
![alt text](images\dog.png)