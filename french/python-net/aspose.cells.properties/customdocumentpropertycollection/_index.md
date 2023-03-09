---
title: CustomDocumentPropertyCollection classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 40
url: /fr/python-net/aspose.cells.properties/customdocumentpropertycollection/
is_root: false
---
##  CustomDocumentPropertyCollection classe
Une collection de propriétés de document personnalisées.



**Héritage:** [CustomDocumentPropertyCollection](/cells/python-net/aspose.cells.properties/customdocumentpropertycollection) → 
[DocumentPropertyCollection](/cells/fr/python-net/aspose.cells.properties/documentpropertycollection)



Le type CustomDocumentPropertyCollection expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [capacity](/cells/fr/python-net/aspose.cells.properties/customdocumentpropertycollection/capacity) | Obtient ou définit le nombre d'éléments que la liste de tableaux peut contenir.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [index_of(name)](/cells/fr/python-net/aspose.cells.properties/customdocumentpropertycollection/index_of/#str) | Obtient l'index d'une propriété par son nom.|
| [index_of(item, index)](/cells/fr/python-net/aspose.cells.properties/customdocumentpropertycollection/index_of/#DocumentProperty-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui s'étend de l'index spécifié au dernier élément.|
| [index_of(item, index, count)](/cells/fr/python-net/aspose.cells.properties/customdocumentpropertycollection/index_of/#DocumentProperty-int-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui commence à l'index spécifié et contient le nombre d'éléments spécifié.|
| [copy_to(array)](/cells/fr/python-net/aspose.cells.properties/customdocumentpropertycollection/copy_to/#list) | Copie la totalité de la liste de tableaux dans une liste de tableaux unidimensionnelle compatible, en commençant au début de la liste de tableaux cible.|
| [copy_to(index, array, array_index, count)](/cells/fr/python-net/aspose.cells.properties/customdocumentpropertycollection/copy_to/#int-list-int-int) |Copie une plage d'éléments de la liste de tableaux vers une liste de tableaux unidimensionnelle compatible, en commençant à l'index spécifié de la liste de tableaux cible.|
| [last_index_of(item)](/cells/fr/python-net/aspose.cells.properties/customdocumentpropertycollection/last_index_of/#DocumentProperty) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la liste complète du tableau.|
| [last_index_of(item, index)](/cells/fr/python-net/aspose.cells.properties/customdocumentpropertycollection/last_index_of/#DocumentProperty-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui s'étend du premier élément à l'index spécifié.|
| [last_index_of(item, index, count)](/cells/fr/python-net/aspose.cells.properties/customdocumentpropertycollection/last_index_of/#DocumentProperty-int-int) |Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui contient le nombre d'éléments spécifié et se termine à l'index spécifié.|
| [add(name, value)](/cells/fr/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-str) | Crée une nouvelle propriété de document personnalisée du**PropertyType.String** Type de données.|
| [add(name, value)](/cells/fr/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-int) | Crée une nouvelle propriété de document personnalisée du**PropertyType.Number** Type de données.|
| [add(name, value)](/cells/fr/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-DateTime) | Crée une nouvelle propriété de document personnalisée du**PropertyType. DateTime** Type de données.|
| [add(name, value)](/cells/fr/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-bool) | Crée une nouvelle propriété de document personnalisée du**PropertyType.Booléen** Type de données.|
| [add(name, value)](/cells/fr/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-float) | Crée une nouvelle propriété de document personnalisée du**Type de propriété. Float** Type de données.|
| [binary_search(item)](/cells/fr/python-net/aspose.cells.properties/customdocumentpropertycollection/binary_search/#DocumentProperty) | Recherche un élément dans toute la liste de tableaux triés à l'aide du comparateur par défaut et renvoie l'index de base zéro de l'élément.|
| [add_link_to_content(name, source)](/cells/fr/python-net/aspose.cells.properties/customdocumentpropertycollection/add_link_to_content/#str-str) | Crée une nouvelle propriété de document personnalisée qui établit un lien vers le contenu.|
| [update_linked_property_value()](/cells/fr/python-net/aspose.cells.properties/customdocumentpropertycollection/update_linked_property_value/#) |Mettez à jour la valeur de la propriété de document personnalisée liée au contenu.|
| [update_linked_range()](/cells/fr/python-net/aspose.cells.properties/customdocumentpropertycollection/update_linked_range/#) | Mettez à jour la valeur de la propriété du document personnalisé sur la plage liée.|



###  Remarques

Chaque objet [DocumentProperty](/cells/fr/python-net/aspose.cells.properties/documentproperty) représente une propriété personnalisée d'un document conteneur.

###  Exemples

```python
from aspose.cells import Workbook

# Instantiate a Workbook object
workbook = Workbook("book1.xls")
# Retrieve a list of all custom document properties of the Excel file
customProperties = workbook.worksheets.custom_document_properties

```

###  Voir également
* module [aspose.cells.properties](..)
* classe [CustomDocumentPropertyCollection](/cells/fr/python-net/aspose.cells.properties/customdocumentpropertycollection)
* classe [DocumentProperty](/cells/fr/python-net/aspose.cells.properties/documentproperty)
* classe [DocumentPropertyCollection](/cells/fr/python-net/aspose.cells.properties/documentpropertycollection)
