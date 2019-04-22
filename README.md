# SparqlP

Este Software es una copia del servidor SPARQL de Apache Jena Fuseki adaptado para guardar la base de datos ttl del proyecto noSQL.
Software original https://jena.apache.org/documentation/fuseki2/index.html#download-fuseki

###  Instrucciones

1. Descargar el repositorio 
2. Ejecutar el archivo fuseki-server.bat
3. Dirigirse a la dirección http://localhost:3030/dataset.html?tab=query&ds=/CancerDB
4. Ejecutar la siguiente consulta

```
  SELECT (count(distinct ?authors) as ?Authors_Count)
  WHERE {
      ?s <http://www.w3.org/1999/02/22-rdf-syntax-ns#Authors> ?authors
  }
```
5. La consulta debe arrojar el sguiente resultado:

```
<a href="https://github.com/AndresDPG/SparqlP.git/master/query.png"><img src="https://github.com/AndresDPG/SparqlP.git/master/query.png" /></a>
```
