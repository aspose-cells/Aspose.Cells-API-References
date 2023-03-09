---
title: metodo is_chart_data_changed
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 70
url: /it/python-net/aspose.cells.charts/chart/is_chart_data_changed/
is_root: false
---
##  is_chart_data_changed() {#}
Rileva se l'origine dati di un grafico è cambiata.


###  ritorna

Restituisce vero se il grafico è cambiato altrimenti restituisce falso


```python
def is_chart_data_changed(self):
    ...
```


###  Osservazioni

Il metodo rileva le modifiche nell'origine dati del grafico prima di eseguire il rendering del grafico in formato immagine.
Alla prima chiamata a Chart.toImage, verranno registrati i dati di origine del grafico (ad es. XValuesParseData, ValuesParseData).
Prima di chiamare nuovamente il metodo Chart.toImage, chiama il metodo IsChartDataChanged per verificare se Chart necessita di un nuovo rendering.


###  Guarda anche
* modulo [aspose.cells.charts](../../)
* classe [Chart](/cells/it/python-net/aspose.cells.charts/chart)
