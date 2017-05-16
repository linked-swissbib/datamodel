# Entity *organisation*

Definition: a record describing an organisation from the real world, who generally acts
* as an author for a bibliographic resource (corporate or meeting), or
* as a library owning an item accessible in swissbib.

## URI schema
```sh
http://data.swissbib.ch/organisation/[ID]
```
## RDF class

| class | use |
| --- | --- |
| [foaf:Organization](http://xmlns.com/foaf/0.1/Organization) | for all resources |

## Properties

| property | use* | datatype | content |
| --- | --- | --- | --- |
| [rdfs:label](http://www.w3.org/2000/01/rdf-schema#label) | everywhere | string | Name of the organisation |

\* The use in every resource doesn't exclude some exceptions. It means that every resource should contain this data.