# Entity *bibliographicResource*

Definition: a bibliographic record, describing a real world object, like a book, an article, a journal, etc. The equivalent of the FRBR manifestation.

## URI schema
```sh
http://data.swissbib.ch/bibliographicResource/[ID]
```

## RDF class

| class | use |
| --- | --- |
| [dct:BibliographicResource](http://purl.org/dc/terms/BibliographicResource) | for all resources |
| [bibo:Article](http://purl.org/ontology/bibo/Article) | for journal articles |
| [bibo:Book](http://purl.org/ontology/bibo/Book) | for monographes |
| [bibo:Manuscript](http://purl.org/ontology/bibo/Manuscript) | for manuscripts |
| [bibo:Periodical](http://purl.org/ontology/bibo/Periodical) | for periodicals (journals, revues, etc.) |
| [bibo:Proceedings](http://purl.org/ontology/bibo/Proceedings) | for conference proceedings |
| [bibo:Series](http://purl.org/ontology/bibo/Series) | for series, collections |
| [bibo:Thesis](http://purl.org/ontology/bibo/Thesis) | for thesis and dissertations |
| [bibo:Website](http://purl.org/ontology/bibo/Website) | for websites |

## Properties

| property | use* | datatype | content |
| --- | --- | --- | --- |
| [bf:instanceOf](http://bibframe.org/vocab/instanceOf) | where possible | URI | Work(s) of which the resource is an instance (Swissbib URI from entity [*work*](http://data.swissbib.ch/work) ) |
| [bibo:edition](http://purl.org/ontology/bibo/edition) | where possible | string | Edition statement and responsibility statement |
| [bibo:isbn10](http://purl.org/ontology/bibo/isbn10) | where possible | string | ISBN in 13 digits |
| [bibo:isbn13](http://purl.org/ontology/bibo/isbn13) | where possible | string | ISBN in 10 characters |
| [bibo:issn](http://purl.org/ontology/bibo/issn) | where possible | string | ISSN |
| [dbo:originalLanguage](http://dbpedia.org/ontology/originalLanguage) | where possible | URI | Original anguage of the resource (Lexvo URI) |
| [dc:format](http://purl.org/dc/elements/1.1/format) | where possible | string | Physical description (extent, other physical details, dimensions, accompanying material) |
| [dct:alternative](http://purl.org/dc/terms/alternative) | where possible | string | Alternative title (incl. number and name of part)|
| [dct:bibliographicCitation](http://purl.org/dc/terms/bibliographicCitation) | where possible | string | Series statement or note about host item |
| [dct:contributor](http://purl.org/dc/terms/contributor) | where possible | URI | Main or secondary author(s) (Swissbib URI from entity [*person*](http://data.swissbib.ch/person) or [*organisation*](http://data.swissbib.ch/organisation)) |
| [dct:hasPart](http://purl.org/dc/terms/hasPart) | where possible | string | Parts of the resource (i.e. titles, ev. statements of responsibility and numbering) |
| [dct:isPartOf](http://purl.org/dc/terms/isPartOf) | where possible | URI | Host item, mainly used for journal articles (Swissbib URI from entity [*bibliographicResource*](http://data.swissbib.ch/bibliographicResource)) |
| [dct:issued](http://purl.org/dc/terms/issued) | every resource | string | Publication date or period |
| [dct:language](http://purl.org/dc/terms/language) | every resource | URI | Language(s) of the resource (Lexvo URI) |
| [dct:subject](http://purl.org/dc/terms/subject) | where possible | URI | Subject(s) (GND URI) |
| [dct:title](http://purl.org/dc/terms/title) | everywhere | string | Title (incl. subtitle, number and name of part) |
| [rdau:P60049](http://www.rdaregistry.info/Elements/u/#P60049) | where possible | URI | RDA content type |
| [rdau:P60050](http://www.rdaregistry.info/Elements/u/#P60050) | where possible | URI | RDA media type |
| [rdau:P60051](http://www.rdaregistry.info/Elements/u/#P60051) | only for serials and integrating resources | URI | RDA mode of issuance |
| [rdau:P60163](http://www.rdaregistry.info/Elements/u/#P60163) | every resource | URI | Country of publication, for some data also Swiss canton of publication (Geonames URI) |
| [rdau:P60333](http://www.rdaregistry.info/Elements/u/#P60333) | where possible | string | Imprint (place of publication, publisher, date) |
| [rdau:P60339](http://www.rdaregistry.info/Elements/u/#P60339) | where possible | string | Statement of responsibility |
| [rdau:P60470](http://www.rdaregistry.info/Elements/u/#P60470) | where possible | string | General note about the resource |
| [rdau:P60489](http://www.rdaregistry.info/Elements/u/#P60489) | where possible | string | Note about the dissertation or thesis |
| [rdfs:isDefinedBy](http://www.w3.org/2000/01/rdf-schema#isDefinedBy) | everywhere | URI | Document describing the bibliographic record (Swissbib URI from entity [*document*](http://data.swissbib.ch/document)) |

\* The use in every resource doesn't exclude some exceptions. It means that every resource should contain this data.
