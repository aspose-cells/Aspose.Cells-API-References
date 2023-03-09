---
title: start_row méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 60
url: /fr/python-net/aspose.cells/lightcellsdataprovider/start_row/
is_root: false
---
##  start_row(row) {#Row}
Commence à enregistrer les données d'une ligne.



```python
def start_row(self, row):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| row | [Row](/cells/fr/python-net/aspose.cells/row) | Objet de ligne à implémenter pour remplir les données. Son index de ligne est la valeur renvoyée du dernier appel de [LightCellsDataProvider.next_row()](/cells/fr/python-net/aspose.cells/lightcellsdataprovider/next_row).<br/>Si la ligne a été initialisée dans le modèle de cellules internes, l'objet ligne existant sera utilisé.<br/> Sinon, un objet Row temporaire sera utilisé pour l'implémentation afin de remplir les données.|
###  Remarques

Il sera appelé au début de l'enregistrement d'une ligne et de ses données de cellules.
Si la ligne actuelle a des propriétés personnalisées telles que la hauteur, le style, etc.,
l'implémentation doit définir ces propriétés sur l'objet Row donné ici.


###  Voir également
* module [aspose.cells](../../)
* classe [LightCellsDataProvider](/cells/fr/python-net/aspose.cells/lightcellsdataprovider)
