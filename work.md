# Entity *work*

Definition: an abstract entity, gathering all bibliographic records with similar characteristics (ex.: same title, same authors, ...). 
At the moment this entity does not match the definitions of the [FRBR work] (https://archive.ifla.org/VII/s13/frbr/frbr_current_toc.htm) or [BIBFRAME work] (https://www.loc.gov/bibframe/docs/bibframe2-model.html).

## URI schema
```sh
http://data.swissbib.ch/work/[ID]
```
## RDF class

| class | use |
| --- | --- |
| [bf:Work](http://bibframe.org/vocab/Work) | for all resources |

## Properties

| property | use* | datatype | content |
| --- | --- | --- | --- |
| [bf:hasInstance](http://bibframe.org/vocab/hasInstance) | everywhere | URI | Bibliographic resource(s) associated to this work (Swissbib URI from entity [*bibliographicResource*](http://data.swissbib.ch/bibliographicResource)) |
| [dct:contributor](http://purl.org/dc/terms/contributor) | where possible | URI | Main or secondary author(s) (Swissbib URI from entity [*person*](http://data.swissbib.ch/person) or [*organisation*](http://data.swissbib.ch/organisation)) |
| [dct:title](http://purl.org/dc/terms/title) | everywhere | string | Title(s) (including possible variants) |

\* The use in every resource doesn't exclude some exceptions. It means that every resource should contain this data.