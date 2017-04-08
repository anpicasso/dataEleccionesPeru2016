# Elecciones Perú 2016 Data / 2016 Peru Elections Data
 - Data de las elecciones generales del 2016 en Perú extraída directamente de la web de la ONPE.
 - Data from 2016 peruvian general elections, extracted directly from ONPE's web.
 
# Formato de la Data
Departamentos
-------------
```
CODE TYPE NAME
010000 P AMAZONAS
020000 P ANCASH
...

Type = P or E; P from Peru, E from Exterior.
```
Provincias
----------
```
codigo tipo nombre
010200 P BAGUA
010300 P BONGARA
...
```
Distritos
----------
```
codigo tipo nombre
010202 P ARAMANGO
010205 P BAGUA
...
```
Local Votación
--------------
```
codigo codigoDistrito nombre
0033 010202 IE 16201
0032 010202 IE MIGUEL MONTEZA TAFUR
...
```
Mesas Votacion
--------------
```
codigo codigoLocalVotacion codigoDistrito
000169 0033 010202
000170 0033 010202
...
```
Actas Votacion
--------------
```
codigoMesa codigoDistrito votosMaximos votosTotales [1..10](Votos por partido] votosBlancos votosNulos
000169 010202 298 210 58 5 1 83 2 24 4 20 0 2 0 11
000170 010202 298 219 44 18 0 89 4 26 7 13 3 1 1 13
...
```
Partidos Políticos
--------------
```
id nombre
1 FRENTE ESPERANZA
2 FUERZA POPULAR
...
```


Extraer y Parsear la data / Extract and parse Data
--------------------------------------------------
 - [Link repositorio / Link repository](https://github.com/anpicasso/extractParseDataONPE)
