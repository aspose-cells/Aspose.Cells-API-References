---
title: is_chart_data_changed Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 70
url: /de/python-net/aspose.cells.charts/chart/is_chart_data_changed/
is_root: false
---
##  is_chart_data_changed() {#}
Erkennt, ob sich die Datenquelle eines Diagramms geändert hat.


###  Kehrt zurück

Gibt „true“ zurück, wenn sich das Diagramm geändert hat, ansonsten „false“.


```python
def is_chart_data_changed(self):
    ...
```


###  Bemerkungen

Die Methode erkennt die Änderungen in der Datenquelle des Diagramms, bevor das Diagramm in das Bildformat gerendert wird.
Beim ersten Chart.toImage-Aufruf werden die Chart-Quelldaten (zB XValuesParseData, ValuesParseData) aufgezeichnet.
Bevor Sie die Chart.toImage-Methode erneut aufrufen, rufen Sie die IsChartDataChanged-Methode auf, um zu prüfen, ob Chart erneut gerendert werden muss.


###  Siehe auch
* Modul [aspose.cells.charts](../../)
* Klasse [Chart](/cells/de/python-net/aspose.cells.charts/chart)
