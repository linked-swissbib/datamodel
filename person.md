# Entity *person*

Definition: a record describing a person from the real world, who generally acts as an author for a bibliographic resource

## URI schema
```sh
http://data.swissbib.ch/person/[ID]
```

## RDF class

| class | use |
| --- | --- |
| [foaf:Person](http://xmlns.com/foaf/0.1/Person) | for all resources |

## Properties

| property | use* | datatype | content |
| --- | --- | --- | --- |
| [dbp:birthYear](http://dbpedia.org/ontology/birthYear) | where possible | gYear | Birth year |
| [dbp:deathYear](http://dbpedia.org/ontology/deathYear) | where possible | gYear | Death year |
| [foaf:firstName](http://xmlns.com/foaf/0.1/firstName) | where possible | string | First name |
| [foaf:lastName](http://xmlns.com/foaf/0.1/lastName) | where possible | string | Last name |
| [foaf:name](http://xmlns.com/foaf/0.1/name) | where possible | string | Name (only if the person has no distinct first and last names) |
| [rdfs:label](http://www.w3.org/2000/01/rdf-schema#label) | everywhere | string | Full heading of the person, including name and - if available - numeration, years of birth/death and title |
| [skos:note](http://www.w3.org/2004/02/skos/core#note ) | where possible | string | Titles and words associated with the name of the person |
| [owl:sameAs](http://www.w3.org/2002/07/owl#sameAs) | where possible | URI | Interconnection between swissbib and DBpedia/VIAF|
| *Properties imported from DBpedia and VIAF >>* ||||
| [dbp:abstract](http://dbpedia.org/ontology/abstract) | where possible | RDF resource (blank node) | Introducing text about the person (one blank node for each language: de, en, fr, it) |
| [dbp:birthDate](http://dbpedia.org/ontology/birthDate) | where possible | date | Birth date |
| [dbp:birthPlace](http://dbpedia.org/ontology/birthPlace) | where possible | URI | Birth place - county and/or city (URI from DBpedia) |
| [dbp:deathDate](http://dbpedia.org/ontology/deathDate) | where possible | date | Death date |
| [dbp:deathPlace](http://dbpedia.org/ontology/deathPlace) | where possible | URI | Death place - county and/or city (URI from DBpedia) |
| [dbp:genre](http://dbpedia.org/ontology/genre) | where possible | URI | Genre (ex: thriller, pop music, poetry, ...) associated with the person (URI from DBpedia) |
| [dbp:influenced](http://dbpedia.org/ontology/influenced) | where possible | URI | Persons or works which were influenced by this person (URI from DBpedia) |
| [dbp:influencedBy](http://dbpedia.org/ontology/influencedBy) | where possible | URI | Other person having influenced this person (URI from DBpedia) |
| [dbp:movement](http://dbpedia.org/ontology/movement) | where possible | URI | artistic movement or school with which the person is associated (URI from DBpedia) |
| [dbp:nationality](http://dbpedia.org/ontology/nationality) | where possible | URI | Nationality (URI from DBpedia) |
| [dbp:notableWork](http://dbpedia.org/ontology/notableWork) | where possible | URI | Notable works of the person (URI from DBpedia) |
| [dbp:occupation](http://dbpedia.org/ontology/occupation) | where possible | URI | Occupation, activity of the person (URI from DBpedia) |
| [dbp:partner](http://dbpedia.org/ontology/partner) | where possible | URI | Partner (URI from DBpedia) |
| [dbp:pseudonym](http://dbpedia.org/ontology/pseudonym) | where possible | URI | Pseudonym |
| [dbp:spouse](http://dbpedia.org/ontology/spouse) | where possible | URI | Spouse (URI from DBpedia) |
| [dbp:thumbnail](http://dbpedia.org/ontology/thumbnail) | where possible | URI | Thumbnail (URI from DBpedia) |
| [schema:alternateName](http://schema.org/givenName) | where possible | string | Alias |
| [schema:birthDate](http://schema.org/birthDate) | where possible | string | Birth date |
| [schema:deathDate](http://schema.org/deathDate) | where possible | string | Death date |
| [schema:familyName](http://schema.org/familyName) | where possible | string | Last name / Family name |
| [schema:gender](http://schema.org/gender) | where possible | string | Gender |
| [schema:givenName](http://schema.org/givenName) | where possible | string | First name / Given name |
| [schema:sameAs](http://schema.org/sameAs) | where possible | URI | URL of a reference web page |
| *Properties imported from DBpedia as literals, content in German, French, Italian and English >>* ||||
| lsb:dbpBirthPlaceAsLiteral | where possible | string | Birth place - county and/or city |
| lsb:dbpDeathPlaceAsLiteral | where possible | string | Death place - county and/or city |
| lsb:dbpGenreAsLiteral | where possible | string | Genre (ex: thriller, pop music, poetry, ...) associated with the person |
| lsb:dbpInfluencedAsLiteral | where possible | string | Persons or works which were influenced by this person |
| lsb:dbpInfluencedByAsLiteral | where possible | string | Other person having influenced this person |
| lsb:dbpMovementAsLiteral | where possible | string | artistic movement or school with which the person is associated |
| lsb:dbpNationalityAsLiteral | where possible | string | Nationality |
| lsb:dbpNotableWorkAsLiteral | where possible | string | Notable works of the person |
| lsb:dbpOccupationAsLiteral | where possible | string | Occupation, activity of the person |
| lsb:dbpPartnerAsLiteral | where possible | string | Partner |
| lsb:dbpSpouseAsLiteral | where possible | string | Spouse |

\* The use in every resource doesn't exclude some exceptions. It means that every resource should contain this data.