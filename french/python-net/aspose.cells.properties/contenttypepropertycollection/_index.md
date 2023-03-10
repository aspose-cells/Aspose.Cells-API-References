---
title: ContentTypePropertyCollection classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 30
url: /fr/python-net/aspose.cells.properties/contenttypepropertycollection/
is_root: false
---
##  ContentTypePropertyCollection classe
Une collection d'objets [ContentTypeProperty](/cells/fr/python-net/aspose.cells.properties/contenttypeproperty) qui représentent des informations supplémentaires.



Le type ContentTypePropertyCollection expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [capacity](/cells/fr/python-net/aspose.cells.properties/contenttypepropertycollection/capacity) | Obtient ou définit le nombre d'éléments que la liste de tableau peut contenir.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [add(name, value)](/cells/fr/python-net/aspose.cells.properties/contenttypepropertycollection/add/#str-str) | Ajoute des informations sur les propriétés du type de contenu.|
| [add(name, value, type)](/cells/fr/python-net/aspose.cells.properties/contenttypepropertycollection/add/#str-str-str) | Ajoute des informations sur les propriétés du type de contenu.|
| [copy_to(array)](/cells/fr/python-net/aspose.cells.properties/contenttypepropertycollection/copy_to/#list) | Copie la totalité de la liste de tableaux dans une liste de tableaux unidimensionnelle compatible, en commençant au début de la liste de tableaux cible.|
| [copy_to(index, array, array_index, count)](/cells/fr/python-net/aspose.cells.properties/contenttypepropertycollection/copy_to/#int-list-int-int) |Copie une plage d'éléments de la liste de tableaux vers une liste de tableaux unidimensionnelle compatible, en commençant à l'index spécifié de la liste de tableaux cible.|
| [index_of(item, index)](/cells/fr/python-net/aspose.cells.properties/contenttypepropertycollection/index_of/#ContentTypeProperty-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui s'étend de l'index spécifié au dernier élément.|
| [index_of(item, index, count)](/cells/fr/python-net/aspose.cells.properties/contenttypepropertycollection/index_of/#ContentTypeProperty-int-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui commence à l'index spécifié et contient le nombre d'éléments spécifié.|
| [last_index_of(item)](/cells/fr/python-net/aspose.cells.properties/contenttypepropertycollection/last_index_of/#ContentTypeProperty) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la liste complète du tableau.|
| [last_index_of(item, index)](/cells/fr/python-net/aspose.cells.properties/contenttypepropertycollection/last_index_of/#ContentTypeProperty-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui s'étend du premier élément à l'index spécifié.|
| [last_index_of(item, index, count)](/cells/fr/python-net/aspose.cells.properties/contenttypepropertycollection/last_index_of/#ContentTypeProperty-int-int) |Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui contient le nombre d'éléments spécifié et se termine à l'index spécifié.|
| [binary_search(item)](/cells/fr/python-net/aspose.cells.properties/contenttypepropertycollection/binary_search/#ContentTypeProperty) | Recherche un élément dans toute la liste de tableaux triés à l'aide du comparateur par défaut et renvoie l'index de base zéro de l'élément.|



###  Exemple

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Add a new property.
workbook.content_type_properties.add("Admin", "Aspose", "text")
# Save the Excel file
workbook.save("book1.xlsm")

```

###  Voir également
* module [aspose.cells.properties](..)
* classe [ContentTypeProperty](/cells/fr/python-net/aspose.cells.properties/contenttypeproperty)
