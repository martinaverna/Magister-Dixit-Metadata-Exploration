# Magister Dixit Metadata Exploration
*Exploring bibliographic metadata from the Magister Dixit Collection*

## About the project
This project is based on the full KU Leuven Libraries [Magister Dixit Collection Dataset](https://github.com/KULeuvenDigitalisering/Magister-Dixit-Collection-Dataset), which is an open dataset available for reuse. <br>
The repository includes a modified version of the **CSV file** from the complete dataset - a description for which can be found below - and a **Jupyter Notebook**.<br>

The Magister Dixit Metadata Exploration lets users explore the bibliographic metadata of Lecture Notes of the Old University of Leuven (XV-XVIII century), particularly focusing on a specific aspect of the metadata, that is, the professional categories who took part in the manuscript production (students, professors, engravers, printers, illustrators…).

## Who can use it
The repository is meant as an example of creative reuses, data visualisations and algorithmic processing of the Magister Dixit Collection. It is designated - on its turn - as a free resource for digital humanities research and engagement.

# The Magister Dixit "Professional Groups" dataset
The Magister_Dixit_professional_groups.csv is a “customized” version of the [Magister_Dixit_Collection_Dataset.csv](https://raw.githubusercontent.com/KULeuvenDigitalisering/Magister-Dixit-Collection-Dataset/master/Magister_Dixit_Collection_Dataset.csv) created by modifying the original dataset with the open source application OpenRefine. 
<br>

**Technical Aspects**<br>
The CSV file (Magister_Dixit_professional_groups.csv) contains 552 records in rows and 31 columns with the following metadata:

| Column | Content type | Instance | Description/MARC 21 reference |
|-|-|-|-|
| 1 | Record ID | 9985450340101488 | Unique key = record id in original cataloging system |
| 2 | URL Limo | https://limo.libis.be/primo-explore/search?query=any,contains,9985450340101488&tab=all_content_tab&search_scope=ALL_CONTENT&vid=KULeuven | Direct url to record in Limo |
| 3 | Date type | m | Encoded indication of type of date, https://www.loc.gov/marc/bibliographic/bd008a.html |
| 4 | Date 1 | 1613 | Date of creation |
| 5 | Date 2 | 1616 | Date of end |
| 6 | Main title | Scripta de sacramentis | Field 246 13: $a main title of the publication https://www.loc.gov/marc/bibliographic/bd245.html |
| 7 | Varying title(s) | Dialectices sive Manuductio ad logicam Lovaniensem ::: Dialectices <br>sive Manuductio ad logicam Lovaniensem a Reverendo in Christo Patro Francisco Vrancx F. M. prædicatore ac Phil: Professore Scripta a Peril: P. F. Eq: D. R: D: L: &orum &orum Die aprilis 24 | https://www.loc.gov/marc/bibliographic/bd246.html#:~:text=Varying%20forms%20of%20the%20title,further%20identification%20of%20the%20item. |
| 8 | Physical extent | 341 p.$bill. | Field 300: $a Description of physical object, varying parameters depending on the nature of the objects, https://www.loc.gov/marc/bibliographic/bd300.html |
| 9 | Binding | Parchment binding ; manuscript title in black ink "[...] Scripta de sacramentis Viggers" ; remnants of ties | https://www.loc.gov/marc/bibliographic/bd563.html |
| 10 | Description of graphic material | \\$ePaper | Material and colors of graphic material, https://www.loc.gov/marc/bibliographic/bd340.html |
| 11 | General notes | Title created by cataloguer ::: F. 0r : Ad usum fratris Leonardi Bosch | https://www.loc.gov/marc/bibliographic/bd500.html |
| 12 | Details | Tractatus sine dictata commentaria in primam partem secundae angelici doctoris$gf. 0r-278v :::* Praefatio$gf. 1r :::* Nota tractatus de beatitudine$gf. 1r-39v :::* Tractatus secundus$gf. 40r-77r :::* Tractatus de libero arbitrio$gf. 77r-119r :::* Tractatus de conscientia$gf. 119r-157v :::* Tractatus de peccatis$gf. 158r-278v ::: Tractatus de sacramentis [incomplete?]$g1*r-10*v | https://www.loc.gov/marc/bibliographic/bd505.html |
| 13 | Genre/form | Manuscripts ::: Lecture notes | https://www.loc.gov/marc/archive/2009-2010/concise/bibliographic/bd655.html |
| 14 | Illustrations | f. 1/3r :$bengraved titlepage$cMetaphysica, Physica, with signs of the Lily, the Falcon, the Castle and the Pig ::: \\$af. 1/30v : pasted on$bengraving(s)$cportrait of a lady ::: f. 1/121v : pasted on$bengraving(s)$cportrait of a veiled lady with book ::: f. 1/128r : pasted on$bengraving(s)$cMusica ::: f. 2/1r :$bengraved titlepage$cMetaphysica, Physica, with signs of the Lily, the Falcon, the Castle and the Pig ::: f. 2/1r : page with$bornamental initials | https://www.loc.gov/marc/bibliographic/bd008b.html |
| 15 | Contributors | Malderus, Joannes$cbishop of Antwerp$d1563-1633$4pfs ::: Mercier, Jean$d? - 1570$4pfs ::: Viggers, Joannes$4pfs ::: Vanden Dael, Paulus$4stu ::: Bosch, Leonardus$4stu ::: Cuyckius, Leonardus$4stu ::: Wierix, Jeronimus$d1553-1619$4egr ::: de Mallery, Charles$d1571-after 1635$gFlemish engraver, active in Antwerpen and Paris$4egr | 700: ‘Personal names’ and its sub-fields https://www.loc.gov/marc/bibliographic/bd700.html |
| 16 | Professor | Malderus, Joannes $cbishop of Antwerp $d1563-1633 ::: Mercier, Jean $d? - 1570 ::: Viggers, Joannes | 700: ‘Personal names’ sorted by sub-field ‘$pfs’ |
| 17 | Student | Vanden Dael, Paulus ::: Bosch, Leonardus ::: Cuyckius, Leonardus | 700: ‘Personal names’ sorted by sub-field ‘$stu’ |
| 18 | Author original work | de Ferrière, Claude Joseph $d1680?-1748? | 700: ‘Personal names’ sorted by sub-field ‘$aow’ |
| 19 | Other | Melchior Stralensis | 700: ‘Personal names’ sorted by sub-field ‘$oth’ |
| 20 | Printer | de Gosen, Hieronymus Iacobus | 700: ‘Personal names’ sorted by sub-field ‘$prt’ |
| 21 | Engraver | Wierix, Jeronimus$d1553-1619 ::: de Mallery, Charles $d1571-after 1635 $gFlemish engraver, active in Antwerpen and Paris | 700: ‘Personal names’ sorted by sub-field ‘$egr’ |
| 22 | Illustrator | Gravelot, Hubert François $d1699-1773 $gFrench book illustrator, engraver, draughtsman and painter | 700: ‘Personal names’ sorted by sub-field ‘$ill’ |
| 23 | Etcher | Harrewijn, François $d1700-1764 $gFlemish etcher, bookseller ::: Denique, Petrus Augustinus $cLeuven $d1721?-1769 | 700: ‘Personal names’ sorted by sub-field ‘$etc’ |
| 24 | Adapter | Haye, Michael $d?-1676 $gFlemish printmaker, draftsman and publisher | 700: ‘Personal names’ sorted by sub-field ‘$adp’ |
| 25 | Artist | Rubens, Peter Paul $d1577-1640 ::: Titiaan $dca. 1485-1576 $gItalian painter | 700: ‘Personal names’ sorted by sub-field ‘$art’ |
| 26 | Place of production 1 | Leuven (Louvain) Pedagogie onbekend | Field 952: $d place, $e name of Pedagogy (in Dutch) https://www.loc.gov/marc/bibliographic/bd264.html |
| 27 | Place of production 2 | Faculty of Arts, pedagogy unknown | Field 952:  $f name of  Pedagogy  in English and Latin  |
| 28 | IE | IE5052929 |  |
| 29 | URL | http://resolver.libis.be/IE5052929/representation | Direct url to image viewer |
| 30 | Label | Abdij van Berne Heeswijk Ms. F11 | Physical object location |
| 31 | Collection | BERNE HEESWIJK | Library collection |

The data processing of the original data set consisted in the following actions:<br>
- removal of columns: ‘Country’, ‘Language’, ‘Content_type’, ‘Media_type’, ‘Carrier_type’, ‘ODIS’;
- creation of new columns: ‘Professor’, ‘Student’, ‘Author_original_work’, ‘Other’, ‘Printer’, ‘Engraver’, ‘Illustrator’, ‘ Etcher’, ‘Adapter’, ‘Artist’ whose content is based on role specifications included in column ‘Contributors’ (MARC sub-field $4);
- removal of MARC field representation positioned in beginning of string (“00$” and “\\$a”) and addition of white spacing between subfields in the same string in order to enhance legibility.

# The Magister Dixit Jupyter Notebook
The Magister Dixit Jupyter Notebook is offered as a tool for exploring and analysing the Magister Dixit metadata collection. It is meant to be reproduced and used as inspiration for further data visualisations and algorithmic processing of the Magister Dixit metadata. <br>
An executable version of the notebook can also be accessed through [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/martinaverna/Magister-Dixit-Metadata-Exploration/master?filepath=Magister-Dixit-Jupyter-Notebook.ipynb) (click on the widget and wait some seconds for the repository to load).

## Cite this repository
When referring to or using the data repository in research publications and documentation, consider citing it with its digital object identifier (DOI) that is minted in Zenodo. <br> 
Cite the original dataset as: KU Leuven Libraries, Digitisation Department. (2020). Magister Dixit Collection [Dataset]. Zenodo. http://doi.org/10.5281/zenodo.3973116. <br>
Cite this repository as: Martina Verna. (2020). Magister Dixit Metadata Exploration. Zenodo. 

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3973116.svg)](https://doi.org/10.5281/zenodo.3973116)  [![DOI](https://zenodo.org/badge/281373610.svg)](https://zenodo.org/badge/latestdoi/281373610)

## Project Attribution
The project was created by **Martina Verna** as part of her thesis project for KU Leuven’s [Advanced Master in Digital Humanities](https://onderwijsaanbod.kuleuven.be/opleidingen/e/CQ_52330579.htm#activetab=diploma_omschrijving): <br> 
Martina Verna, *Digital Heritage Collections as Open Data. Exploring methods and tools for publishing bibliographic metadata and promoting their use*, KU Leuven Master of Digital Humanities (2019-2020).


