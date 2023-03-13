---
title: start_sheet méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 70
url: /fr/python-net/aspose.cells/lightcellsdataprovider/start_sheet/
is_root: false
---
##  start_sheet(sheet_index) {#int}
Démarre l'enregistrement d'une feuille de calcul.


###  Retour

true si ce fournisseur fournira des données pour la feuille donnée ; false si la feuille donnée doit utiliser son modèle de données normal (Cells).


```python
def start_sheet(self, sheet_index):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| sheet_index | int | index de la feuille courante à sauvegarder.|
###  Remarques

Il sera appelé au début de l'enregistrement d'une feuille de calcul lors de l'enregistrement d'un classeur.
 Si le fournisseur doit se référer à*`sheetIndex`* plus tard
dans la méthode startRow(Row) ou startCell(Cell),
 autrement dit, si le processus a besoin de savoir quelle feuille de calcul est en cours de traitement,
 la mise en œuvre doit conserver le*`sheetIndex`* valeur ici.


###  Voir également
* module [aspose.cells](../../)
* classe [LightCellsDataProvider](/cells/fr/python-net/aspose.cells/lightcellsdataprovider)
