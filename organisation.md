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

| property | use* | datatype | content | source |
| --- | --- | --- | --- | --- |
| [dbo:country](http://dbpedia.org/ontology/country) | where possible | URI + labels | Country | Wikidata [wdt:P17](https://www.wikidata.org/wiki/Property:P17), GND [geographicAreaCode](https://d-nb.info/standards/elementset/gnd#geographicAreaCode) |
| [dbo:notableWork](http://dbpedia.org/ontology/notableWork) | where possible | URI + labels | Notable Works as URI | Wikidata [wdt:P800](https://www.wikidata.org/wiki/Property:P800), VIAF [dbo:notableWork](http://dbpedia.org/ontology/notableWork), Dbpedia [dbo:notableWork](http://dbpedia.org/ontology/notableWork) |
| [dbo:thumbnail](http://dbpedia.org/ontology/thumbnail) | where possible | URI |  Image  | Wikidata [wdt:P18](https://www.wikidata.org/wiki/Property:P18), GND [depiction](https://d-nb.info/standards/elementset/gnd#depiction), Dbpedia [dbo:thumbnail](http://dbpedia.org/ontology/thumbnail) |
| [dbo:website](http://dbpedia.org/ontology/website) | where possible | URI |  official website | GND [homepage](https://d-nb.info/standards/elementset/gnd#homepage), Wikidata[wdt:P856](https://www.wikidata.org/wiki/property:wdt:P856) |
| [foaf:primaryTopicOf]() | where possible | URI | Wikipedia Links | GND [wikipedia](https://d-nb.info/standards/elementset/gnd#wikipedia) and Dbpedia [foaf:primaryTopicOf]() |
| [gnd:abbreviatedNameForTheCorporateBody](https://d-nb.info/standards/elementset/gnd#abbreviatedNameForTheCorporateBody) | where possible | string |  | GND [abbreviatedNameForTheCorporateBody](https://d-nb.info/standards/elementset/gnd#abbreviatedNameForTheCorporateBody) |
| [gnd:benefactor](https://d-nb.info/standards/elementset/gnd#benefactor) | where possible | URI + labels | 	A person, family, or corporate body being the benefactor of a work, a thing, or a corporate body | GND [benefactor](https://d-nb.info/standards/elementset/gnd#benefactor) |
| [gnd:biographicalOrHistoricalInformation](https://d-nb.info/standards/elementset/gnd#biographicalOrHistoricalInformation) | where possible | string |  | GND [biographicalOrHistoricalInformation](https://d-nb.info/standards/elementset/gnd#biographicalOrHistoricalInformation) |
| [gnd:broaderTermGeneral](https://d-nb.info/standards/elementset/gnd#broaderTermGeneral) | where possible | URI + labels |  | GND [broaderTermGeneral](https://d-nb.info/standards/elementset/gnd#broaderTermGeneral) |
| [gnd:broaderTermInstantial](https://d-nb.info/standards/elementset/gnd#broaderTermInstantial) | where possible | URI + labels |  | GND [broaderTermInstantial](https://d-nb.info/standards/elementset/gnd#broaderTermInstantial) |
| [gnd:broaderTermPartitive](https://d-nb.info/standards/elementset/gnd#broaderTermPartitive) | where possible | URI + labels |  | GND [broaderTermPartitive](https://d-nb.info/standards/elementset/gnd#broaderTermPartitive) |
| [gnd:celebratedCorporateBody](https://d-nb.info/standards/elementset/gnd#celebratedCorporateBody) | where possible | URI + labels |   | GND [celebratedCorporateBody](https://d-nb.info/standards/elementset/gnd#celebratedCorporateBody) |
| [gnd:celebratedPerson](https://d-nb.info/standards/elementset/gnd#celebratedPerson) | where possible | URI + labels |  | GND [celebratedPerson](https://d-nb.info/standards/elementset/gnd#celebratedPerson) |
| [gnd:collector](https://d-nb.info/standards/elementset/gnd#collector) | where possible | URI + labels |  | GND [collector](https://d-nb.info/standards/elementset/gnd#collector) |
| [gnd:complexSeeReferenceSubject](https://d-nb.info/standards/elementset/gnd#complexSeeReferenceSubject) | where possible | URI + labels |  | GND [complexSeeReferenceSubject](https://d-nb.info/standards/elementset/gnd#complexSeeReferenceSubject) |
| [gnd:contributingCorporateBody](https://d-nb.info/standards/elementset/gnd#contributingCorporateBody) | where possible | URI + labels |   | GND [contributingCorporateBody](https://d-nb.info/standards/elementset/gnd#contributingCorporateBody) |
| [gnd:contributingPerson](https://d-nb.info/standards/elementset/gnd#contributingPerson) | where possible | URI + labels |  | GND [contributingPerson](https://d-nb.info/standards/elementset/gnd#contributingPerson) |
| [gnd:contributingPlaceOrGeographicName](https://d-nb.info/standards/elementset/gnd#contributingPlaceOrGeographicName) | where possible | URI + labels |  | GND [contributingPlaceOrGeographicName](https://d-nb.info/standards/elementset/gnd#contributingPlaceOrGeographicName) |
| [gnd:corporateBodyIsMember](https://d-nb.info/standards/elementset/gnd#corporateBodyIsMember) | where possible | URI + labels |  | GND [corporateBodyIsMember](https://d-nb.info/standards/elementset/gnd#corporateBodyIsMember) |
| [gnd:curator](https://d-nb.info/standards/elementset/gnd#curator) | where possible | URI + labels |  | GND [curator](https://d-nb.info/standards/elementset/gnd#curator) |
| [gnd:dateOfConferenceOrEvent](https://d-nb.info/standards/elementset/gnd#dateOfConferenceOrEvent) | where possible | string |  | GND [dateOfConferenceOrEvent](https://d-nb.info/standards/elementset/gnd#dateOfConferenceOrEvent) |
| [gnd:dateOfEstablishment](https://d-nb.info/standards/elementset/gnd#dateOfEstablishment) | where possible | string |  | GND [dateOfEstablishment](https://d-nb.info/standards/elementset/gnd#dateOfEstablishment) |
| [gnd:dateOfEstablishmentAndTermination](https://d-nb.info/standards/elementset/gnd#dateOfEstablishmentAndTermination) | where possible | string |  | GND [dateOfEstablishmentAndTermination](https://d-nb.info/standards/elementset/gnd#dateOfEstablishmentAndTermination) |
| [gnd:dateOfTermination](https://d-nb.info/standards/elementset/gnd#dateOfTermination) | where possible | string |  | GND [dateOfTermination](https://d-nb.info/standards/elementset/gnd#dateOfTermination) |
| [gnd:definition](https://d-nb.info/standards/elementset/gnd#definition) | where possible | string |  | GND [definition](https://d-nb.info/standards/elementset/gnd#definition) |
| [gnd:deprecatedUri](https://d-nb.info/standards/elementset/gnd#deprecatedUri) | where possible | URI |  | GND [deprecatedUri](https://d-nb.info/standards/elementset/gnd#deprecatedUri) |
| [gnd:exhibitor](https://d-nb.info/standards/elementset/gnd#exhibitor) | where possible | URI + labels |  | GND [exhibitor](https://d-nb.info/standards/elementset/gnd#exhibitor) |
| [gnd:fieldOfActivity](https://d-nb.info/standards/elementset/gnd#fieldOfActivity) | where possible | string |  | GND [fieldOfActivity](https://d-nb.info/standards/elementset/gnd#fieldOfActivity) |
| [gnd:founder](https://d-nb.info/standards/elementset/gnd#founder) | where possible | URI + labels |  | GND [founder](https://d-nb.info/standards/elementset/gnd#founder) |
| [gnd:gndIdentifier](https://d-nb.info/standards/elementset/gnd#gndIdentifier) | where possible | string |  | GND [gndIdentifier](https://d-nb.info/standards/elementset/gnd#gndIdentifier) |
| [gnd:gndSubjectCategory](https://d-nb.info/standards/elementset/gnd#gndSubjectCategory) | where possible | URI + labels |  | GND [gndSubjectCategory](https://d-nb.info/standards/elementset/gnd#gndSubjectCategory) |
| [gnd:hierarchicalSuperiorOfTheConferenceOrEvent](https://d-nb.info/standards/elementset/gnd#hierarchicalSuperiorOfTheConferenceOrEvent) | where possible | URI + labels |  | GND [hierarchicalSuperiorOfTheConferenceOrEvent](https://d-nb.info/standards/elementset/gnd#hierarchicalSuperiorOfTheConferenceOrEvent) |
| [gnd:hierarchicalSuperiorOfTheCorporateBody](https://d-nb.info/standards/elementset/gnd#hierarchicalSuperiorOfTheCorporateBody) | where possible | URI + labels | parent organization | GND [hierarchicalSuperiorOfTheCorporateBody](https://d-nb.info/standards/elementset/gnd#hierarchicalSuperiorOfTheCorporateBody), Wikidata[wdt:P749](https://www.wikidata.org/wiki/property:wdt:P749) |
| [gnd:languageCode](https://d-nb.info/standards/elementset/gnd#languageCode) | where possible | URI + labels |  | GND [languageCode](https://d-nb.info/standards/elementset/gnd#languageCode) |
| [gnd:musician](https://d-nb.info/standards/elementset/gnd#musician) | where possible | URI + labels |  | GND [musician](https://d-nb.info/standards/elementset/gnd#musician) |
| [gnd:occasionOfTheSubjectHeading](https://d-nb.info/standards/elementset/gnd#occasionOfTheSubjectHeading) | where possible | URI + labels |   | GND [occasionOfTheSubjectHeading](https://d-nb.info/standards/elementset/gnd#occasionOfTheSubjectHeading) |
| [gnd:oldAuthorityNumber](https://d-nb.info/standards/elementset/gnd#oldAuthorityNumber) | where possible | string |  | GND [oldAuthorityNumber](https://d-nb.info/standards/elementset/gnd#oldAuthorityNumber) |
| [gnd:precedingConferenceOrEvent](https://d-nb.info/standards/elementset/gnd#precedingConferenceOrEvent) | where possible | URI + labels | follows (other event) / event | GND [precedingConferenceOrEvent](https://d-nb.info/standards/elementset/gnd#precedingConferenceOrEvent), Wikidata[wdt:P155](https://www.wikidata.org/wiki/property:wdt:P155) |
| [gnd:precedingCorporateBody](https://d-nb.info/standards/elementset/gnd#precedingCorporateBody) | where possible | URI + labels |  | GND [precedingCorporateBody](https://d-nb.info/standards/elementset/gnd#precedingCorporateBody) |
| [gnd:publication](https://d-nb.info/standards/elementset/gnd#publication) | where possible | string |  | GND [publication](https://d-nb.info/standards/elementset/gnd#publication) |
| [gnd:relatedConferenceOrEvent](https://d-nb.info/standards/elementset/gnd#relatedConferenceOrEvent) | where possible | URI + labels |  | GND [relatedConferenceOrEvent](https://d-nb.info/standards/elementset/gnd#relatedConferenceOrEvent) |
| [gnd:relatedCorporateBody](https://d-nb.info/standards/elementset/gnd#relatedCorporateBody) | where possible | URI + labels |  | GND [relatedCorporateBody](https://d-nb.info/standards/elementset/gnd#relatedCorporateBody) |
| [gnd:relatedPerson](https://d-nb.info/standards/elementset/gnd#relatedPerson) | where possible | URI + labels |  | GND [relatedPerson](https://d-nb.info/standards/elementset/gnd#relatedPerson) |
| [gnd:relatedPlaceOrGeographicName](https://d-nb.info/standards/elementset/gnd#relatedPlaceOrGeographicName) | where possible | URI + labels |  | GND [relatedPlaceOrGeographicName](https://d-nb.info/standards/elementset/gnd#relatedPlaceOrGeographicName) |
| [gnd:relatedSubjectHeading](https://d-nb.info/standards/elementset/gnd#relatedSubjectHeading) | where possible | URI + labels |  | GND [relatedSubjectHeading](https://d-nb.info/standards/elementset/gnd#relatedSubjectHeading) |
| [gnd:relatedTerm](https://d-nb.info/standards/elementset/gnd#relatedTerm) | where possible | URI + labels |  | GND [relatedTerm](https://d-nb.info/standards/elementset/gnd#relatedTerm) |
| [gnd:relatedWork](https://d-nb.info/standards/elementset/gnd#relatedWork) | where possible | URI + labels |  | GND [relatedWork](https://d-nb.info/standards/elementset/gnd#relatedWork) |
| [gnd:spatialAreaOfActivity](https://d-nb.info/standards/elementset/gnd#spatialAreaOfActivity) | where possible | URI + labels |  | GND [spatialAreaOfActivity](https://d-nb.info/standards/elementset/gnd#spatialAreaOfActivity) |
| [gnd:sponsorOrPatron](https://d-nb.info/standards/elementset/gnd#sponsorOrPatron) | where possible | URI + labels |  | GND [sponsorOrPatron](https://d-nb.info/standards/elementset/gnd#sponsorOrPatron) |
| [gnd:succeedingConferenceOrEvent](https://d-nb.info/standards/elementset/gnd#succeedingConferenceOrEvent) | where possible | URI + labels | followed by (other event) /event | GND [succeedingConferenceOrEvent](https://d-nb.info/standards/elementset/gnd#succeedingConferenceOrEvent), Wikidata[wdt:P156](https://www.wikidata.org/wiki/property:wdt:P156) |
| [gnd:succeedingCorporateBody](https://d-nb.info/standards/elementset/gnd#succeedingCorporateBody) | where possible | URI + labels |  | GND [succeedingCorporateBody](https://d-nb.info/standards/elementset/gnd#succeedingCorporateBody) |
| [gnd:succeedingPlaceOrGeographicName](https://d-nb.info/standards/elementset/gnd#succeedingPlaceOrGeographicName) | where possible | URI + labels |  | GND [succeedingPlaceOrGeographicName](https://d-nb.info/standards/elementset/gnd#succeedingPlaceOrGeographicName) |
| [gnd:temporaryNameOfTheConferenceOrEvent](https://d-nb.info/standards/elementset/gnd#temporaryNameOfTheConferenceOrEvent) | where possible | string |  | GND [temporaryNameOfTheConferenceOrEvent](https://d-nb.info/standards/elementset/gnd#temporaryNameOfTheConferenceOrEvent) |
| [gnd:temporaryNameOfTheCorporateBody](https://d-nb.info/standards/elementset/gnd#temporaryNameOfTheCorporateBody) | where possible | string |  | GND [temporaryNameOfTheCorporateBody](https://d-nb.info/standards/elementset/gnd#temporaryNameOfTheCorporateBody) |
| [gnd:topic](https://d-nb.info/standards/elementset/gnd#topic) | where possible | string |  | GND [topic](https://d-nb.info/standards/elementset/gnd#topic) |
| [owl:sameAs](http://www.w3.org/2002/07/owl#sameAs) | where possible | URI | URIs in other datasets | swissbib, VIAF, GND, Wikidata and DBpedia |
| [rdfs:label](http://www.w3.org/2000/01/rdf-schema#label) | everywhere | string | Full heading of the person, including name and - if available - numeration, years of birth/death and title | GND 
| [schema:alternateName](http://schema.org/alternateName) | where possible | string | alternate names for the organisation | 
| [schema:description](http://schema.org/description) | where possible | string (de, en, fr, it) | description|  |
| [schema:endDate](http://schema.org/endDate) | where possible | string | end time (when this event took place) / event | Wikidata [wdt:P582](https://www.wikidata.org/wiki/Property:P582), VIAF [schema:endDate](http://schema.org/endDate) |
| [schema:location](http://schema.org/location) | where possible | URI + labels |  | GND [placeOfConferenceOrEvent](https://d-nb.info/standards/elementset/gnd#placeOfConferenceOrEvent), VIAF [schema:location](http://schema.org/location) |
| [schema:location](http://schema.org/) | where possible | URI + labels | headquarters location | GND [placeOfBusiness](https://d-nb.info/standards/elementset/gnd#placeOfBusiness), Wikidata [wdt:P159](https://www.wikidata.org/wiki/Property:P159), VIAF [schema:location](http://schema.org/location) |
| [schema:name](http://schema.org/name) | where possible | string |  |  |
| [schema:organizer](http://schema.org/organizer) | where possible | URI + labels | Organizer / event | Wikidata [wdt:P664](https://www.wikidata.org/wiki/Property:P664), GND [organizerOrHost](https://d-nb.info/standards/elementset/gnd#organizerOrHost) |
| [schema:startDate](http://schema.org/startDate) | where possible | string | start time (when this event took place) / event | Wikidata [wdt:P580](https://www.wikidata.org/wiki/Property:P580), VIAF [schema:startDate](http://schema.org/startDate) |
| [wdt:P1037](https://www.wikidata.org/wiki/Property:P1037) | where possible | URI + labels | director / manager | Wikidata [wdt:P1037](https://www.wikidata.org/wiki/Property:wdt:P1037) |
| [wdt:P1082](https://www.wikidata.org/wiki/Property:P1082) | where possible | URI + labels | population | Wikidata [wdt:P1082](https://www.wikidata.org/wiki/Property:wdt:P1082) |
| [wdt:P1132](https://www.wikidata.org/wiki/Property:P1132) | where possible | URI + labels | number of participants / event | Wikidata [wdt:P1132](https://www.wikidata.org/wiki/Property:wdt:P1132) |
| [wdt:P131](https://www.wikidata.org/wiki/Property:P131) | where possible | URI + labels | located in admin territory | Wikidata [wdt:P131](https://www.wikidata.org/wiki/Property:wdt:P131) |
| [wdt:P136](https://www.wikidata.org/wiki/Property:P136) | where possible | URI + labels | genre  | Wikidata [wdt:P136](https://www.wikidata.org/wiki/Property:wdt:P136) |
| [wdt:P137](https://www.wikidata.org/wiki/Property:P137) | where possible | URI + labels | operator | Wikidata [wdt:P137](https://www.wikidata.org/wiki/Property:wdt:P137) |
| [wdt:P1454](https://www.wikidata.org/wiki/Property:P1454) | where possible | URI + labels | legal form | Wikidata [wdt:P1454](https://www.wikidata.org/wiki/Property:wdt:P1454) |
| [wdt:P179](https://www.wikidata.org/wiki/Property:P179) | where possible | URI + labels | part of the series /event | Wikidata [wdt:P179](https://www.wikidata.org/wiki/Property:wdt:P179) |
| [wdt:P2046](https://www.wikidata.org/wiki/Property:P2046) | where possible | URI + labels | area | Wikidata [wdt:P2046](https://www.wikidata.org/wiki/Property:wdt:P2046) |
| [wdt:P2348](https://www.wikidata.org/wiki/Property:P2348) | where possible | URI + labels | time period / event | Wikidata [wdt:P2348](https://www.wikidata.org/wiki/Property:wdt:P2348) |
| [wdt:P242](https://www.wikidata.org/wiki/Property:P242) | where possible | URI + labels | locator map image | Wikidata [wdt:P242](https://www.wikidata.org/wiki/Property:wdt:P242) |
| [wdt:P276](https://www.wikidata.org/wiki/Property:P276) | where possible | URI + labels | location | Wikidata [wdt:P276](https://www.wikidata.org/wiki/Property:wdt:P276) |
| [wdt:P281](https://www.wikidata.org/wiki/Property:P281) | where possible | URI + labels | postal code | Wikidata [wdt:P281](https://www.wikidata.org/wiki/Property:wdt:P281) |
| [wdt:P31](https://www.wikidata.org/wiki/Property:P31) | where possible | URI + labels | instance of  | Wikidata [wdt:P31](https://www.wikidata.org/wiki/Property:wdt:P31) |
| [wdt:P36](https://www.wikidata.org/wiki/Property:P36) | where possible | URI + labels | Capital | Wikidata [wdt:P36](https://www.wikidata.org/wiki/Property:wdt:P36) |
| [wdt:P361](https://www.wikidata.org/wiki/Property:P361) | where possible | URI + labels | part of / event | Wikidata [wdt:P361](https://www.wikidata.org/wiki/Property:wdt:P361) |
| [wdt:P373](https://www.wikidata.org/wiki/Property:P373) | where possible | URI + labels | Commons category | Wikidata [wdt:P373](https://www.wikidata.org/wiki/Property:wdt:P373) |
| [wdt:P393](https://www.wikidata.org/wiki/Property:P393) | where possible | URI + labels | edition number (of event) / event | Wikidata [wdt:P393](https://www.wikidata.org/wiki/Property:wdt:P393) |
| [wdt:P421](https://www.wikidata.org/wiki/Property:P421) | where possible | URI + labels | located in time zone | Wikidata [wdt:P421](https://www.wikidata.org/wiki/Property:wdt:P421) |
| [wdt:P473](https://www.wikidata.org/wiki/Property:P473) | where possible | URI + labels | local dialing code | Wikidata [wdt:P473](https://www.wikidata.org/wiki/Property:wdt:P473) |
| [wdt:P495](https://www.wikidata.org/wiki/Property:P495) | where possible | URI + labels | country of origin | Wikidata [wdt:P495](https://www.wikidata.org/wiki/Property:wdt:P495) |
| [wdt:P527](https://www.wikidata.org/wiki/Property:P527) | where possible | URI + labels | has part (inverse of 'part of') / event | Wikidata [wdt:P527](https://www.wikidata.org/wiki/Property:wdt:P527) |
| [wdt:P571](https://www.wikidata.org/wiki/Property:P571) | where possible | URI + labels | inception | Wikidata [wdt:P571](https://www.wikidata.org/wiki/Property:wdt:P571) |
| [wdt:P576](https://www.wikidata.org/wiki/Property:P576) | where possible | URI + labels | dissolved. abolished or demolished | Wikidata [wdt:P576](https://www.wikidata.org/wiki/Property:wdt:P576) |
| [wdt:P625](https://www.wikidata.org/wiki/Property:P625) | where possible | URI + labels | coordinate location | Wikidata [wdt:P625](https://www.wikidata.org/wiki/Property:wdt:P625) |
| [wdt:P6375](https://www.wikidata.org/wiki/Property:P6375) | where possible | URI + labels | located at street address | Wikidata [wdt:P6375](https://www.wikidata.org/wiki/Property:wdt:P6375) |
| [wdt:P710](https://www.wikidata.org/wiki/Property:P710) | where possible | URI + labels | Participant / event | Wikidata [wdt:P710](https://www.wikidata.org/wiki/Property:wdt:P710) |
| [wdt:P791](https://www.wikidata.org/wiki/Property:P791) | where possible | URI + labels | International Standard Identifier for Libraries (ISIL)  | Wikidata [wdt:P791](https://www.wikidata.org/wiki/Property:wdt:P791) |
| [wdt:P968](https://www.wikidata.org/wiki/Property:P968) | where possible | URI + labels | email address | Wikidata [wdt:P968](https://www.wikidata.org/wiki/Property:wdt:P968) |
| [wdt:P973](https://www.wikidata.org/wiki/Property:P973) | where possible | URI + labels | described at URL / event | Wikidata [wdt:P973](https://www.wikidata.org/wiki/Property:wdt:P973) |

\* The use in every resource doesn't exclude some exceptions. It means that every resource should contain this data.