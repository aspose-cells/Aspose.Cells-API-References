---
title: clear méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 30
url: /fr/python-net/aspose.cells/externallinkcollection/clear/
is_root: false
---
##  clear() {#}
Supprime tous les liens externes.



```python
def clear(self):
    ...
```


###  Remarques

Lors de la suppression des liens externes, toutes les formules qui y font référence seront également supprimées car
les références deviennent invalides.

##  clear(update_references_as_local) {#bool}
Supprime tous les liens externes.



```python
def clear(self, update_references_as_local):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| update_references_as_local | bool | Si mettre à jour toutes les références de liens externes en tant que références du classeur actuel lui-même.|
###  Remarques

Si les références doivent être mises à jour, les références aux liens externes dans les formules seront remplacées par le classeur actuel.
Par exemple, la formule d'origine d'une cellule est "='externalsource.xlam'!customfunction()",
après avoir supprimé les liens externes, la formule deviendra "=customfunction()".
Si les références ne doivent pas être mises à jour, toutes les formules avec des références à des liens externes
seront également supprimés car ces références deviennent invalides.


###  Voir également
* module [aspose.cells](../../)
* classe [ExternalLinkCollection](/cells/fr/python-net/aspose.cells/externallinkcollection)
