---
title: remove_at méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 40
url: /fr/python-net/aspose.cells/externallinkcollection/remove_at/
is_root: false
---
##  remove_at(index) {#int}
Supprime le lien externe spécifié du classeur.



```python
def remove_at(self, index):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| index | int | l'index du lien externe à supprimer.|
###  Remarques

Lors de la suppression du lien externe, toutes les formules qui y font référence seront également supprimées car
les références deviennent invalides.

##  remove_at(index, update_references_as_local) {#int-bool}
Supprime le lien externe spécifié du classeur.



```python
def remove_at(self, index, update_references_as_local):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| index | int | l'index du lien externe à supprimer.|
| update_references_as_local | bool | Si mettre à jour toutes les références du lien externe donné à la référence du classeur actuel lui-même.|
###  Remarques

Si les références doivent être mises à jour, les références aux liens externes dans les formules seront remplacées par le classeur actuel.
Par exemple, le lien externe à supprimer est "externalsource.xlam" et il définit une fonction personnalisée "customfunction()",
la formule originale d'une cellule est "='externalsource.xlam'!customfunction()",
après avoir supprimé la formule deviendra "=customfunction()".
Si la référence ne doit pas être mise à jour, toutes les formules faisant référence à ce lien externe
seront également supprimés car ces références deviennent invalides.


###  Voir également
* module [aspose.cells](../../)
* classe [ExternalLinkCollection](/cells/fr/python-net/aspose.cells/externallinkcollection)
