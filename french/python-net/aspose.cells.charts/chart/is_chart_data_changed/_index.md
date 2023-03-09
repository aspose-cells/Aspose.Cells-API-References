---
title: is_chart_data_changed méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 70
url: /fr/python-net/aspose.cells.charts/chart/is_chart_data_changed/
is_root: false
---
##  is_chart_data_changed() {#}
Détecte si la source de données d'un graphique a changé.


###  Retour

Renvoie true si le graphique a changé sinon renvoie false


```python
def is_chart_data_changed(self):
    ...
```


###  Remarques

La méthode détecte les changements dans la source de données du graphique avant de rendre le graphique au format image.
Au premier appel de Chart.toImage, les données source du graphique (par exemple XValuesParseData, ValuesParseData) seront enregistrées.
Avant d'appeler à nouveau la méthode Chart.toImage, appelez la méthode IsChartDataChanged pour vérifier si Chart doit être restitué.


###  Voir également
* module [aspose.cells.charts](../../)
* classe [Chart](/cells/fr/python-net/aspose.cells.charts/chart)
