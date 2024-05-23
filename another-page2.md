---
layout: default
---

# SPARQL QUERIES


## Are there any military uniforms in the clothing description ontology?
```js
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX arco: <https://w3id.org/arco/ontology/arco/>
PREFIX a-cd: <https://w3id.org/arco/ontology/clothing-description/>
PREFIX agent: <https://w3id.org/arco/resource/Agent/>
SELECT *
WHERE {
?Clothing
rdfs:label ?label 
FILTER(REGEX(?label, "uniforme, militare"))
}
LIMIT 3
```

## Which are 15  clothes cataloged by the agency Soprintendenza Archeologia, belle arti e paesaggio per il Comune di Napoli and Museo Storico Italiano della Guerra onlus?
```js
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX arco: <https://w3id.org/arco/ontology/arco/>
PREFIX a-cd: <https://w3id.org/arco/ontology/clothing-description/>
PREFIX agent: <https://w3id.org/arco/resource/Agent/>
SELECT *
WHERE {
?Clothing
rdfs:label ?label 
{ ?Clothing  arco:hasCataloguingAgency agent:2d700f56ee050c27059505c6d73c6be5 }
UNION
{ ?Clothing arco:hasCataloguingAgency agent:30c1084f5edbacf14dcfc486ad94005d }
}
LIMIT 15
```

## Which are 15 clothes cataloged by the agency Soprintendenza Archeologia, belle arti e paesaggio per il Comune di Napoli and Museo Storico Italiano della Guerra onlus? Without duplicate results
```js
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX arco: <https://w3id.org/arco/ontology/arco/>
PREFIX a-cd: <https://w3id.org/arco/ontology/clothing-description/>
PREFIX agent: <https://w3id.org/arco/resource/Agent/>
SELECT DISTINCT?Clothing
WHERE {
?Clothing
rdfs:label ?label 
{ ?Clothing  arco:hasCataloguingAgency agent:2d700f56ee050c27059505c6d73c6be5 }
UNION
{ ?Clothing arco:hasCataloguingAgency agent:30c1084f5edbacf14dcfc486ad94005d }
}
LIMIT 15
```

## Which are 15 clothes cataloged by the agency Soprintendenza Archeologia, belle arti e paesaggio per il Comune di Napoli and Museo Storico Italiano della Guerra onlus? Without duplicate results. For all retrieved clothings provide the depiction if any is available.
```js
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX arco: <https://w3id.org/arco/ontology/arco/>
PREFIX a-cd: <https://w3id.org/arco/ontology/clothing-description/>
PREFIX agent: <https://w3id.org/arco/resource/Agent/>
SELECT DISTINCT?Clothing
WHERE {
?Clothing
rdfs:label ?label 
{ ?Clothing  arco:hasCataloguingAgency agent:2d700f56ee050c27059505c6d73c6be5 }
UNION
{ ?Clothing arco:hasCataloguingAgency agent:30c1084f5edbacf14dcfc486ad94005d }
OPTIONAL { ?clothing a-cd:depiction ?depiction }
}
LIMIT 15
```

## Which are 15 clothes cataloged by the agency Soprintendenza Archeologia, belle arti e paesaggio per il Comune di Napoli and Museo Storico Italiano della Guerra onlus? Without duplicate results ordered in a descending way. For all retrieved clothings provide the depiction if any is available.
```js
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX arco: <https://w3id.org/arco/ontology/arco/>
PREFIX a-cd: <https://w3id.org/arco/ontology/clothing-description/>
PREFIX agent: <https://w3id.org/arco/resource/Agent/>
SELECT DISTINCT?Clothing
WHERE {
?Clothing
rdfs:label ?label 
{ ?Clothing  arco:hasCataloguingAgency agent:2d700f56ee050c27059505c6d73c6be5 }
UNION
{ ?Clothing arco:hasCataloguingAgency agent:30c1084f5edbacf14dcfc486ad94005d }
OPTIONAL { ?clothing a-cd:depiction ?depiction }
}
ORDER BY DESC (?Clothing)
LIMIT 15
```

[back](./)
