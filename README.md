### 8.7.2019 | DH2019 Utrecht

# XML2RDF

## Extracting RDF Statements From XML Resources With XTriples

_Max Grüntgens_ (ORCID: [0000-0001-8736-9393](https://orcid.org/0000-0001-8736-9393))

_Thomas Kollatz_ (ORCID: [0000-0003-1904-1841](https://orcid.org/0000-0003-1904-1841))

## Description

The tutorial focuses on scholars, who want to acquaint themselves with a “low threshold” — generic, simple yet powerful, and explorative — workflow of modelling, extracting, processing (queries, visualizations), and publishing of “structured data” (LOD, Semantic Web) from heterogeneous XML-sources by means of XPath. The web service used for extraction is [_XTriples_](https://xtriples.lod.academy). The instructors assume basic acquaintance with XML and XPath (both will be quickly revised, “cheat sheets” will be provided).

The tutorial uses research data provided by the API of the scholarly edition _Der Sturm: Digitale Quellenedition zur Geschichte der internationalen Avantgarde_ ([https://sturm-edition.de](https://sturm-edition.de)) by Marjam Trautmann (ORCID: [0000-0003-2423-7144](https://orcid.org/0000-0003-2423-7144)) and Torsten Schrade. The edition provides APIs ecapsulating persons, places, works, letters, and files.

The _XTriples webservice_ was developed by Torsten Schrade (Academy of Sciences and Literature, Mainz, ORCID: [0000-0002-0953-2818](https://orcid.org/0000-0002-0953-2818)). More about XTriples and its usage within the _Digital Humanities_ may be found here: [https://xtriples.lod.academy/dh.html](https://xtriples.lod.academy/dh.html).

The conference abstract of the workshop is available here: [https://dev.clariah.nl/files/dh2019/boa/1073.html](https://dev.clariah.nl/files/dh2019/boa/1073.html).

### Presentation

The presentation slides may be found at [digicademy.github.io/ws-dh2019-xml2rdf](https://digicademy.github.io/ws-dh2019-xml2rdf).

You may clone the repository with Git `git clone https://github.com/digicademy/ws-dh2019-xml2rdf.git` or download the repository as a [ZIP file](https://github.com/digicademy/ws-dh2019-xml2rdf/archive/master.zip).

Below you may find lists collecting the relevant xml source data files, the finished XTriples configuration files for RDF extraction, some  handouts, and a list of important links to sites and services used during the workshop.

#### Input data files (XML)

* [Sturm Letters](https://digicademy.github.io/ws-dh2019-xml2rdf/data/source/sturm_letters.xml)
* [Sturm Persons](https://digicademy.github.io/ws-dh2019-xml2rdf/data/source/sturm_persons.xml)
* [Sturm Places](https://digicademy.github.io/ws-dh2019-xml2rdf/data/source/sturm_places.xml)
* [Sturm Works](https://digicademy.github.io/ws-dh2019-xml2rdf/data/source/sturm_works.xml)

All data source files were aggregated via the public Sturm-Data-APIs. You may find the APIs at [https://sturm-edition.de/ressourcen/schnittstellen.html](https://sturm-edition.de/ressourcen/schnittstellen.html) (German).

#### Xtriples configuration files (XML)

* [XTriples Configuration Letters](https://digicademy.github.io/ws-dh2019-xml2rdf/data/config/sturm_config_letters_xtriples.xml)
* [XTriples Configuration Persons](https://digicademy.github.io/ws-dh2019-xml2rdf/data/config/sturm_config_persons_xtriples.xml)
* [XTriples Configuration Places](https://digicademy.github.io/ws-dh2019-xml2rdf/data/config/sturm_config_places_xtriples.xml)
* [XTriples Configuration Works](https://digicademy.github.io/ws-dh2019-xml2rdf/data/config/sturm_config_works_xtriples.xml)


#### Output data files (XML)

* [Sturm Letters](https://digicademy.github.io/ws-dh2019-xml2rdf/data/output/sturm_output_letters.rdf)
* [Sturm Persons](https://digicademy.github.io/ws-dh2019-xml2rdf/data/output/sturm_output_persons.rdf)
* [Sturm Places](https://digicademy.github.io/ws-dh2019-xml2rdf/data/output/sturm_output_places.rdf)
* [Sturm Works](https://digicademy.github.io/ws-dh2019-xml2rdf/data/output/sturm_output_works.rdf)

#### CSV files

* [artwork.csv](https://digicademy.github.io/ws-dh2019-xml2rdf/data/csv/artwork.csv)
* [mentioned_persons_gender.csv](https://digicademy.github.io/ws-dh2019-xml2rdf/data/csv/mentioned_persons_gender.csv)
* [places_dariah_geobrowser.csv](https://digicademy.github.io/ws-dh2019-xml2rdf/data/csv/places_dariah_geobrowser.csv)

#### Handouts

* 

#### Important links

* XTriples Webservice for RDF-Extraction: [https://xtriples.lod.academy/](https://xtriples.lod.academy/)
* oXygen-Document-Type-Association: [https://oxygen.adwmainz.net/xtriples-configuration/update.xml](https://oxygen.adwmainz.net/xtriples-configuration/update.xml)
* RDF4j Triple Store: [https://rdf4j.adwmainz.net/rdf4j-workbench/](https://rdf4j.adwmainz.net/rdf4j-workbench/)
* Visualization service: [http://app.rawgraphs.io](http://app.rawgraphs.io)
* Person Normdata Webservice: [http://lobid.org/gnd/](http://lobid.org/gnd/)
* Places Normdata Webservice: [https://sws.geonames.org/357994/about.rdf](https://sws.geonames.org/357994/about.rdf) (Example “Egypt”) 

#### Visualizations

* Based on the [get_places.txt](https://digicademy.github.io/ws-dh2019-xml2rdf/data/queries/get_places.txt) SPARQL Query and used within the [Dariah GeoBrowser](https://geobrowser.de.dariah.eu): [https://geobrowser.de.dariah.eu/?csv1=https://geobrowser.de.dariah.eu/storage/735201](https://geobrowser.de.dariah.eu/?csv1=https://geobrowser.de.dariah.eu/storage/735201)
* Based on the [get_artworks.txt](https://digicademy.github.io/ws-dh2019-xml2rdf/data/queries/get_artworks.txt) SPARQL Query and used within [app.rawgraphs.io](http://app.rawgraphs.io/) Alluvial Diagram: [https://digicademy.github.io/ws-dh2019-xml2rdf/data/queries/artworks.png](https://digicademy.github.io/ws-dh2019-xml2rdf/data/queries/artworks.png)
* Based on the [get_gender.txt](https://digicademy.github.io/ws-dh2019-xml2rdf/data/queries/get_gender.txt) SPARQL Query and used within [app.rawgraphs.io](http://app.rawgraphs.io/) Alluvial Diagram: [https://digicademy.github.io/ws-dh2019-xml2rdf/data/queries/gender.png](https://digicademy.github.io/ws-dh2019-xml2rdf/data/queries/gender.png)

<hr/>

Based on the boilerplate at https://github.com/digicademy/impress-js-boilerplate

A live demo of the boilerplate can be found at http://digicademy.github.io/impress-js-boilerplate/

Released under [CC-BY 4.0](https://creativecommons.org/licenses/by/4.0/), @digicademy
