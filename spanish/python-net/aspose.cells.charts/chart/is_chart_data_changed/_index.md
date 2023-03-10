---
title: is_chart_data_changed método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 70
url: /es/python-net/aspose.cells.charts/chart/is_chart_data_changed/
is_root: false
---
##  is_chart_data_changed() {#}
Detecta si la fuente de datos de un gráfico ha cambiado.


###  Devoluciones

Devuelve verdadero si el gráfico ha cambiado; de lo contrario, devuelve falso


```python
def is_chart_data_changed(self):
    ...
```


###  Observaciones

El método detecta los cambios en la fuente de datos del gráfico antes de representar el gráfico en formato de imagen.
En la primera llamada a Chart.toImage, se registrarán los datos de origen del gráfico (p. ej., XValuesParseData, ValuesParseData).
Antes de volver a llamar al método Chart.toImage, llame al método IsChartDataChanged para verificar si Chart necesita volver a renderizarse.


###  Ver también
* módulo [aspose.cells.charts](../../)
* clase [Chart](/cells/es/python-net/aspose.cells.charts/chart)
