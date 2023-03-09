---
title: index_of méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 60
url: /fr/python-net/aspose.cells.properties/customdocumentpropertycollection/index_of/
is_root: false
---
##  index_of(name) {#str}
Obtient l'index d'une propriété par son nom.


###  Retour

L'indice de base zéro. Valeur négative si introuvable.


```python
def index_of(self, name):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| name | str | Nom non sensible à la casse de la propriété.|


##  index_of(item, index) {#DocumentProperty-int}
Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui s'étend de l'index spécifié au dernier élément.


###  Retour

Index de base zéro de la première occurrence de value dans la plage d'éléments de la liste de tableaux qui s'étend de startIndex au dernier élément, s'il est trouvé ; sinon, -1.


```python
def index_of(self, item, index):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| item | [DocumentProperty](/cells/fr/python-net/aspose.cells.properties/documentproperty) | L'objet à localiser dans la liste de tableaux. La valeur peut être nulle.|
| index | int | Index de départ de base zéro de la recherche. 0 (zéro) est valide dans une liste vide.|


##  index_of(item, index, count) {#DocumentProperty-int-int}
Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui commence à l'index spécifié et contient le nombre d'éléments spécifié.


###  Retour

Index de base zéro de la première occurrence de value dans la plage d'éléments de la liste de tableaux qui commence à startIndex et contient le nombre d'éléments, s'il est trouvé ; sinon, -1.


```python
def index_of(self, item, index, count):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| item | [DocumentProperty](/cells/fr/python-net/aspose.cells.properties/documentproperty) | L'objet à localiser dans la liste de tableaux. La valeur peut être nulle.|
| index | int | Index de départ de base zéro de la recherche. 0 (zéro) est valide dans une liste vide.|
| count | int | Le nombre d'éléments dans la section à rechercher.|



###  Voir également
* module [aspose.cells.properties](../../)
* classe [CustomDocumentPropertyCollection](/cells/fr/python-net/aspose.cells.properties/customdocumentpropertycollection)
