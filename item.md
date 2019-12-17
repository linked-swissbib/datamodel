# Entity *item*

Definition: a library item, which is a concrete physical object.

## URI schema
```sh
http://data.swissbib.ch/item/[ID]
```

## RDF class

| class | use |
| --- | --- |
| [bf:HeldItem](http://bibframe.org/vocab/HeldItem) | for all resources |

## Properties

| property | use* | datatype | content |
| --- | --- | --- | --- |
| [bf:holdingFor](http://bibframe.org/vocab/holdingFor) | everywhere | URI | Bibliographic resource associated to this item (Swissbib URI from entity [*bibliographicResource*](http://data.swissbib.ch/bibliographicResource)) |
| [bf:subLocation](http://bibframe.org/vocab/subLocation) | where possible | string | Sublocation within the library |
| [bibo:locator](http://purl.org/ontology/bibo/locator) | where possible | string | Shelfmark |
| [bibo:owner](http://purl.org/ontology/bibo/owner) | everywhere | URI | Library owning the item (Swissbib URI from entity [*organisation*](http://data.swissbib.ch/organisation)) |
| [foaf:page](http://xmlns.com/foaf/spec/#term_page) | everywhere | URI | Link to the item in the local library interface |

\* The use in every resource doesn't exclude some exceptions. It means that every resource should contain this data.