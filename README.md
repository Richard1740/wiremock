# Wiremock

1) Ejecutar en una consola

java -jar wiremock-jre8-standalone-2.33.2.jar --port port --global-response-templating

Por ejemplo: 

java -jar wiremock-jre8-standalone-2.33.2.jar --port 9999 --global-response-templating


2) Abrir un browser y probar las siguientes direcciones: 

a) http://localhost:<port>/get/this (vamos a obtener el mock test.json)

Ejemplo: http://localhost:9999/get/this

Abre una página con el mensaje Here it is!

b) http://localhost:<port>/api/json-data-10min.php?key=demo&locatie=<locación>

Ejemplo: http://localhost:9999/api/json-data-10min.php?key=demo&locatie=Amsterdam

En locatie podemos poner cualquier locación y nos debe devolver la temperatura mockeada para esa locación.
La temperatura (temp) esta configurada para que sea random con cada llamada.
