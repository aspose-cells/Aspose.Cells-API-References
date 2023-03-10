---
title: is_chart_data_changed metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 70
url: /sv/python-net/aspose.cells.charts/chart/is_chart_data_changed/
is_root: false
---
##  is_chart_data_changed() {#}
Upptäcker om ett diagrams datakälla har ändrats.


###  Returnerar

Returnerar sant om diagrammet har ändrats, annars returneras falskt


```python
def is_chart_data_changed(self):
    ...
```


###  Anmärkningar

Metoden upptäcker ändringarna i diagrammets datakälla innan diagrammet återges till bildformat.
Vid första Chart.toImage-anropet kommer diagramkälldata (t.ex. XValuesParseData, ValuesParseData) att registreras.
Innan du anropar metoden Chart.toImage igen, anropa metoden IsChartDataChanged för att kontrollera om diagrammet behöver återrenderas.


###  Se även
* modul [aspose.cells.charts](../../)
* klass [Chart](/cells/sv/python-net/aspose.cells.charts/chart)
