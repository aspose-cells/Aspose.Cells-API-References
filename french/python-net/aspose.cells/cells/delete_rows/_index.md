---
title: delete_rows méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 260
url: /fr/python-net/aspose.cells/cells/delete_rows/
is_root: false
---
##  delete_rows(row_index, total_rows) {#int-int}
Supprime plusieurs lignes.



```python
def delete_rows(self, row_index, total_rows):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| row_index | int | Premier index de ligne à supprimer.|
| total_rows | int | Nombre de lignes à supprimer.|
###  Remarques

Si la plage supprimée contient la partie supérieure (pas entière) de la table (ListObject),
la plage n'a pas pu être supprimée et rien ne sera fait. Cela fonctionne comme MS Excel.

##  delete_rows(row_index, total_rows, update_reference) {#int-int-bool}
Supprime plusieurs lignes dans la feuille de calcul.


###  Retour




```python
def delete_rows(self, row_index, total_rows, update_reference):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| row_index | int | Indice de ligne.|
| total_rows | int | Nombre de lignes à supprimer.|
| update_reference | bool | Indique si la mise à jour des références dans d'autres feuilles de calcul.|



###  Voir également
* module [aspose.cells](../../)
* classe [Cells](/cells/fr/python-net/aspose.cells/cells)
