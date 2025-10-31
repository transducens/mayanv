# MayanV, Mayan-Spanish parallel corpora

This repository contains MayanV, a collection of parallel corpora between several Mayan languages and Spanish. MayanV is introduced in the paper ["Curated Datasets and Neural Models for Machine Translation of Informal Registers between Mayan and Spanish Vernaculars"](https://aclanthology.org/2024.naacl-long.156/), accepted at the 2024 Annual Conference of the North American Chapter of the Association for Computational Linguistics, NAACL2024.

## Erratum
A critial error was discovered in the Tzeltal and Ixil datasets. Consequently, all corresponding experiments have been corrected and repeated. The table below replaces Table 5 in the original paper. The Tzeltal and Ixil datasets have been temporarily removed pending revisions. The revised versions will be reuploaded shortly.

|  | maya-es |  |  |  | es-maya |  |  |  |
|---|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
|  | bilingual |  | multilingual |  | bilingual |  | multilingual |  |
|  | baseline | mayanv | baseline | mayanv | baseline | mayanv | baseline | mayanv |
| acr | - | - | 0,7 | 1,8 | - | - | 0 | 0.1 |
| agu | - | 0 | 0,3 | 1,2 | - | 0 | 0,1 | 0.3 |
| cac | - | 0,1 | 0,1 | 4,5 | - | 0,1 | 0 | 3.8 |
| itz | - | - | 0,6 | 1 | - | - | 0,1 | 0.1 |
| ixl | 0,3 | 8,4 | 0,2 | 7,8 | 0 | 1,3 | 0,1 | 6.1 |
| kek | 0,6 | 7,2 | 2,4 | 10,2 | 1,1 | 8 | 2,8 | 14.0 |
| kjb | - | 3,5 | 0,2 | 5,6 | - | 4 | 0 | 7.3 |
| mam | 0,9 | 3,8 | 1,1 | 3,9 | 0,2 | 1 | 0,4 | 1.4 |
| poc | - | 5,2 | 0,3 | 8,7 | - | 1,8 | 0 | 5.8 |
| poh | - | 0,2 | 1,3 | 5 | - | 0,3 | 2,7 | 2.5 |
| quc | - | 2,9 | 3 | 5,6 | 2,1 | 3,3 | 5,7 | 6.2 |
| qum | - | - | 0,6 | 1,8 | - | - | 0,1 | 0.1 |
| ttc | - | 6,9 | 0,7 | 11,2 | - | 7,1 | 0 | 11.2 |
| tzh | 0.86 | 10.6 | 1,8 | 9,4 | 1.0 | 6.9 | 2,3 | 8.7 |
| tzj | - | 0 | 0,2 | 4,6 | - | 0,1 | 0,1 | 3.5 |

## Included languages

MayanV includes curated parallel corpora for Spanish and the following Mayan languages spoken in Guatemala and Southern Mexico:

| ISO Code | Language    | Words (Mayan) | Words (Spanish) | Sentences |
|----------|-------------|--------------:|----------------:|----------:|
| acr      | Achi        |         6,994 |           7,657 |     1,343 |
| agu      | Awakatec    |         7,325 |           9,700 |     1,930 |
| cac      | Chuj        |         9,398 |          10,916 |     2,299 |
| itz      | Itza’       |         6,069 |           7,512 |     1,539 |
| ixl      | Ixil        |        10,888 |          12,137 |     2,325 |
| kek      | Q’eqchi’    |        18,529 |          21,835 |     4,133 |
| kjb      | Q’anjob’al  |        18,035 |          18,238 |     3,014 |
| mam      | Mam         |        15,453 |          19,117 |     3,093 |
| poc      | Poqomam     |        18,039 |          21,744 |     3,583 |
| poh      | Poqomchi’   |         6,479 |           7,149 |     1,787 |
| quc      | K’iche’     |        14,468 |          15,474 |     2,632 |
| qum      | Sipakapense |         9,780 |           9,328 |     1,356 |
| ttc      | Tektitek    |        23,571 |          24,896 |     4,022 |
| tzh      | Tzeltal     |       103,309 |         128,659 |    19,846 |
| tzj      | Tz’utujil   |        12,283 |          11,404 |     2,519 |

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
