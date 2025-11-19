# MayanV2, Mayan-Spanish parallel corpora

This repository contains MayanV2 (MayanV v2), an annotated collection of parallel corpora between several Mayan languages and Spanish. MayanV (v1) was first introduced in the paper ["Curated Datasets and Neural Models for Machine Translation of Informal Registers between Mayan and Spanish Vernaculars"](https://aclanthology.org/2024.naacl-long.156/), accepted at the 2024 Annual Conference of the North American Chapter of the Association for Computational Linguistics, NAACL2024.

## Changes introduced in v2
MayanV2 is a upgrade from MayanV that introduces additional languages, additional parallel sentences, and diverse annotations, including part-of-speech, inflection, and dialect, whenever these are available. MayanV2 is a further improvement because of the use of enhanced extraction methodology centered around the use of Google's Gemini Pro 2.5 model.

| ISO code 	| Language            	| Sentences 	|  Words (Mayan) 	|
|:--------:	|---------------------	|:---------:	|:------:	|
|    acr   	| Achi                	|    1563   	|  7641  	|
|    agu   	| Awakatek            	|    3094   	|  12512 	|
|  agu_ctk 	| Awakatek/Chalchitek 	|    3319   	|  15452 	|
|    cac   	| Chuj                	|    5763   	|  26881 	|
|    cak   	| Kaqchikel           	|    6227   	|  49148 	|
|    ctk   	| Chalchitek          	|    991    	|  6158  	|
|    itz   	| Itzaʼ               	|    1522   	|  6050  	|
|    ixl   	| Ixil                	|    4571   	|  22769 	|
|    jac   	| Jakaltek/Poptiʼ     	|    4384   	|  26001 	|
|    kek   	| Qʼeqchiʼ            	|   10863   	|  59165 	|
|    kjb   	| Qʼanjobʼal          	|    2987   	|  18432 	|
|    mam   	| Mam                 	|   15229   	| 101706 	|
|    poc   	| Poqomam             	|    3659   	|  18864 	|
|    poh   	| Poqomchiʼ           	|    1746   	|  6544  	|
|    quc   	| Kʼicheʼ             	|    2624   	|  14484 	|
|    qum   	| Sipakapense         	|    1344   	|  9363  	|
|    ttc   	| Tektiteko           	|    3974   	|  24492 	|
|    tzh   	| Tzʼeltal            	| 12733     	| 66227  	|
|    tzj   	| Tzʼutujil           	| 13211     	| 66738  	|

## Documents included in MayanV2
The most important addition to MayanV2 is the inclusion of a collection of previously unreleased dictionaries, whose annotations are included in the corpus. These annotations are not uniform across languages, given the asynchronous publication history and the different language communities and editorial teams involved. The dictionaries, along with the documents included in the previous release, have been extracted using Google Gemini Pro 2.5 and have been meticulously structured and curated using the available metadata. All documents are released as JSON files.

## Erratum
A critical error was discovered in the Tzeltal and Ixil datasets in the previous release. Consequently, all corresponding experiments have been corrected and repeated. See the [erratum]() for additional details.

Sources for each corpus are discussed in the article. The datasets are parallel with Spanish, the dominant language of the region, and are taken from official native sources focused on representing informal, day-to-day, and non-domain-specific language.

## Structure

Each language corpus is organized into its respective folder within the repository. Additionally, each language folder contains its own README file providing details about the resources used to create the corpus. Language folders: [Achi](https://github.com/transducens/mayanv/tree/master/MayanV/acr), [Awakatec](https://github.com/transducens/mayanv/tree/master/MayanV/agu), [Chuj](https://github.com/transducens/mayanv/tree/master/MayanV/cac), [Itza’](https://github.com/transducens/mayanv/tree/master/MayanV/itz), [Ixil](https://github.com/transducens/mayanv/tree/master/MayanV/ixl), [Q’eqchi’](https://github.com/transducens/mayanv/tree/master/MayanV/kek), [Q’anjob’al](https://github.com/transducens/mayanv/tree/master/MayanV/kjb), [Mam](https://github.com/transducens/mayanv/tree/master/MayanV/mam), [Poqomam](https://github.com/transducens/mayanv/tree/master/MayanV/poc), [Poqomchi’](https://github.com/transducens/mayanv/tree/master/MayanV/poh), [K’iche’](https://github.com/transducens/mayanv/tree/master/MayanV/quc), [Sipakapense](https://github.com/transducens/mayanv/tree/master/MayanV/qum), [Tektitek](https://github.com/transducens/mayanv/tree/master/MayanV/ttc), [Tzeltal](https://github.com/transducens/mayanv/tree/master/MayanV/tzh), [Tz’utujil](https://github.com/transducens/mayanv/tree/master/MayanV/tzj).


## Acknowledgments

MayanV has been produced as part of the R+D+i project [Lightweight neural translation technologies for low-resource languages (LiLowLa)](https://transducens.dlsi.ua.es/lilowla/) (PID2021-127999NB-I00) funded by the Spanish Ministry
of Science and Innovation (MCIN), the Spanish Research Agency (AEI/10.13039/501100011033) and the European Regional Development Fund A way to make Europe. 

## License

These data are released under this licensing scheme:
 * We do not own any of the text from which these data has been extracted.
 * We license the actual packaging of these parallel data under the Creative Commons CC0 license ("no rights reserved").

## Citing this work

If you use this dataset as part of your developments, please cite it as follows:

```
@inproceedings{lou-etal-2024-curated,
    title = "Curated Datasets and Neural Models for Machine Translation of Informal Registers between {M}ayan and {S}panish Vernaculars",
    author = "Lou, Andr{\'e}s  and
      P{\'e}rez-Ortiz, Juan Antonio  and
      S{\'a}nchez-Mart{\'\i}nez, Felipe  and
      S{\'a}nchez-Cartagena, V{\'\i}ctor",
    editor = "Duh, Kevin  and
      Gomez, Helena  and
      Bethard, Steven",
    booktitle = "Proceedings of the 2024 Conference of the North American Chapter of the Association for Computational Linguistics: Human Language Technologies (Volume 1: Long Papers)",
    month = jun,
    year = "2024",
    address = "Mexico City, Mexico",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2024.naacl-long.156",
    pages = "2838--2850",
}
```

A `CITATION.cff` file is also included in this repository.
