---
title: process_cell méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 20
url: /fr/python-net/aspose.cells/lightcellsdatahandler/process_cell/
is_root: false
---
##  process_cell(cell) {#Cell}
Commence à traiter une cellule.


###  Retour

si cette cellule doit être conservée dans le modèle de cellules de la feuille actuelle.
Généralement, il doit être faux afin que toutes les cellules ne soient pas conservées en mémoire après avoir été traitées, puis enregistrées en mémoire.
Dans un but particulier, tel que l'utilisateur doit accéder à certaines cellules plus tard après le traitement de l'ensemble du classeur,
l'utilisateur peut faire en sorte que cette méthode renvoie true pour conserver ces cellules spéciales dans le modèle Cells et y accéder ultérieurement par des API telles que Cells[ligne, colonne].
Cependant, conserver les données des cellules dans le modèle Cells nécessitera plus de mémoire et si toutes les cellules sont conservées, la lecture du fichier modèle
en mode LightCells deviendra le même avec une lecture normale.


```python
def process_cell(self, cell):
    ...
```


| Paramètres| Taper| Description|
| :- | :- | :- |
| cell | [Cell](/cells/fr/python-net/aspose.cells/cell) | Cell objet en cours de traitement actuellement|
###  Remarques

Il sera appelé après la lecture des données d'une cellule.


###  Voir également

* module [aspose.cells](../../)
* classe [LightCellsDataHandler](/cells/fr/python-net/aspose.cells/lightcellsdatahandler)
