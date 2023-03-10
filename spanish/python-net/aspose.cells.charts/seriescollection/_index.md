---
title: SeriesCollection clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 240
url: /es/python-net/aspose.cells.charts/seriescollection/
is_root: false
---
##  SeriesCollection clase
Encapsula una colección de [Series](/cells/es/python-net/aspose.cells.charts/series) objetos.



El tipo SeriesCollection expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [category_data](/cells/es/python-net/aspose.cells.charts/seriescollection/category_data) | Obtiene o establece el rango de valores de Axis de categoría.<br/> Puede ser un rango de celdas (como "d1:e10"),<br/> o una secuencia de valores (como,"{2,6,8,10}").|
| [second_category_data](/cells/es/python-net/aspose.cells.charts/seriescollection/second_category_data) | Obtiene o establece el rango de valores de Axis de segunda categoría.<br/> Puede ser un rango de celdas (como "d1:e10"),<br/> o una secuencia de valores (como,"{2,6,8,10}").<br/> Solo efectos cuando algunas ASeries se trazan en el segundo eje.|
| [is_color_varied](/cells/es/python-net/aspose.cells.charts/seriescollection/is_color_varied) | Representa si el color de los puntos es variado.|
| [capacity](/cells/es/python-net/aspose.cells.charts/seriescollection/capacity) | Obtiene o establece el número de elementos que puede contener la lista de matrices.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [add(area, is_vertical)](/cells/es/python-net/aspose.cells.charts/seriescollection/add/#str-bool) | Agrega la colección [SeriesCollection](/cells/es/python-net/aspose.cells.charts/seriescollection) a un gráfico.|
| [add(area, is_vertical, check_labels)](/cells/es/python-net/aspose.cells.charts/seriescollection/add/#str-bool-bool) | Agrega la colección [SeriesCollection](/cells/es/python-net/aspose.cells.charts/seriescollection) a un gráfico.|
| [copy_to(array)](/cells/es/python-net/aspose.cells.charts/seriescollection/copy_to/#list) | Copia toda la lista de matrices en una lista de matrices unidimensional compatible, comenzando por el principio de la lista de matrices de destino.|
| [copy_to(index, array, array_index, count)](/cells/es/python-net/aspose.cells.charts/seriescollection/copy_to/#int-list-int-int) |Copia un rango de elementos de la lista de arreglos a una lista de arreglos unidimensional compatible, comenzando en el índice especificado de la lista de arreglos de destino.|
| [index_of(item, index)](/cells/es/python-net/aspose.cells.charts/seriescollection/index_of/#Series-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el índice especificado hasta el último elemento.|
| [index_of(item, index, count)](/cells/es/python-net/aspose.cells.charts/seriescollection/index_of/#Series-int-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de matriz que comienza en el índice especificado y contiene el número especificado de elementos.|
| [last_index_of(item)](/cells/es/python-net/aspose.cells.charts/seriescollection/last_index_of/#Series) | Busca el objeto especificado y devuelve el índice de base cero de la última aparición en toda la lista de matrices.|
| [last_index_of(item, index)](/cells/es/python-net/aspose.cells.charts/seriescollection/last_index_of/#Series-int) | Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el primer elemento hasta el índice especificado.|
| [last_index_of(item, index, count)](/cells/es/python-net/aspose.cells.charts/seriescollection/last_index_of/#Series-int-int) |Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de matriz que contiene el número especificado de elementos y termina en el índice especificado.|
| [get_series_by_order(order)](/cells/es/python-net/aspose.cells.charts/seriescollection/get_series_by_order/#int) | Obtiene el elemento [Series](/cells/es/python-net/aspose.cells.charts/series) por pedido.|
| [change_series_order(source_index, dest_index)](/cells/es/python-net/aspose.cells.charts/seriescollection/change_series_order/#int-int) | Cambia directamente los órdenes de las dos series.|
| [set_series_names(start_index, area, is_vertical)](/cells/es/python-net/aspose.cells.charts/seriescollection/set_series_names/#int-str-bool) | Establece el nombre de todas las series en el gráfico.|
| [add_r1c1(area, is_vertical)](/cells/es/python-net/aspose.cells.charts/seriescollection/add_r1c1/#str-bool) | Agrega la colección [SeriesCollection](/cells/es/python-net/aspose.cells.charts/seriescollection) a un gráfico.|
| [binary_search(item)](/cells/es/python-net/aspose.cells.charts/seriescollection/binary_search/#Series) | Busca un elemento en toda la lista de matrices ordenadas mediante el comparador predeterminado y devuelve el índice de base cero del elemento.|



###  Ejemplo

```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartType

# Instantiating a Workbook object
workbook = Workbook()
# Adding a new worksheet to the Excel object
sheetIndex = workbook.worksheets.add()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[sheetIndex]
# Adding a sample value to "A1" cell
worksheet.cells.get("A1").put_value(50)
# Adding a sample value to "A2" cell
worksheet.cells.get("A2").put_value(100)
# Adding a sample value to "A3" cell
worksheet.cells.get("A3").put_value(150)
# Adding a sample value to "A4" cell
worksheet.cells.get("A4").put_value(200)
# Adding a sample value to "B1" cell
worksheet.cells.get("B1").put_value(60)
# Adding a sample value to "B2" cell
worksheet.cells.get("B2").put_value(32)
# Adding a sample value to "B3" cell
worksheet.cells.get("B3").put_value(50)
# Adding a sample value to "B4" cell
worksheet.cells.get("B4").put_value(40)
# Adding a sample value to "C1" cell as category data
worksheet.cells.get("C1").put_value("Q1")
# Adding a sample value to "C2" cell as category data
worksheet.cells.get("C2").put_value("Q2")
# Adding a sample value to "C3" cell as category data
worksheet.cells.get("C3").put_value("Y1")
# Adding a sample value to "C4" cell as category data
worksheet.cells.get("C4").put_value("Y2")
# Adding a chart to the worksheet
chartIndex = worksheet.charts.add(ChartType.COLUMN, 5, 0, 15, 5)
# Accessing the instance of the newly added chart
chart = worksheet.charts[chartIndex]
# Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
chart.n_series.add("A1:B4", True)
# Setting the data source for the category data of NSeries
chart.n_series.category_data = "C1:C4"
# Saving the Excel file
workbook.save("book1.xls")

```

###  Ver también
* módulo [aspose.cells.charts](..)
* clase [Series](/cells/es/python-net/aspose.cells.charts/series)
* clase [SeriesCollection](/cells/es/python-net/aspose.cells.charts/seriescollection)
