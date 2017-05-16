# Entity *document*

Definition: a document describing the bibliographic record, i.e. the entity bibliographicResource. Contains statements about the rights, the creator and the creation date of the record itself.

## URI schema
```sh
http://data.swissbib.ch/document/[ID]
```
## RDF class

| class | use |
| --- | --- |
| [bibo:Document](http://purl.org/ontology/bibo/document) | for all resources |

## Properties

| property | use* | datatype | content |
| --- | --- | --- | --- |
| [bf:local](http://bibframe.org/vocab/local) | everywhere | string | Local ID(s) (i.e. from the various data providers of Swissbib) of the bibliographic resource |
| [dc:contributor](http://purl.org/dc/elements/1.1/contributor) | where possible | string | Institution (i.e. library) that created the bibliographic resource (in form of a string if the institution is outside of Switzerland and not known by swissbib) |
| [dct:contributor](http://purl.org/dc/terms/contributor) | where possible | URI | Institution (i.e. library) that created the bibliographic resource (Swissbib URI from entity [*organisation*](http://data.swissbib.ch/organisation)) |
| [dct:issued](http://purl.org/dc/terms/issued) | everywhere | dateTime | Date of publication of the bibliographic resource |
| [dct:modified](http://purl.org/dc/terms/modified) | everywhere | dateTime | Date of last modification of the bibliographic resource |
| [dct:rights](http://purl.org/dc/terms/rights) | where possible | string | Mark "Metadata rights reserved" (should not be visible in the API) |
| [foaf:primaryTopic](http://xmlns.com/foaf/0.1/primaryTopic) | everywhere | URI | Link to the bibliographic resource described (Swissbib URI from entity [*bibliographicResource*](http://data.swissbib.ch/bibliographicResource)) |

\* The use in every resource doesn't exclude some exceptions. It means that every resource should contain this data.