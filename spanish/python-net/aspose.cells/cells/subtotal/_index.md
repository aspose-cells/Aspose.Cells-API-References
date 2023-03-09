---
title: subtotal método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 920
url: /es/python-net/aspose.cells/cells/subtotal/
is_root: false
---
##  subtotal(ca, group_by, function, total_list) {#CellArea-int-ConsolidationFunction-list}
Crea subtotales para el rango.



```python
def subtotal(self, ca, group_by, function, total_list):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| ca | [CellArea](/cells/es/python-net/aspose.cells/cellarea) | El rango|
| group_by | int | El campo por el que agrupar, como un desplazamiento de entero basado en cero|
| function | [ConsolidationFunction](/cells/es/python-net/aspose.cells/consolidationfunction) | La función de subtotales.|
| total_list | list | Una matriz de compensaciones de campo de base cero, que indica los campos a los que se agregan los subtotales.|


##  subtotal(ca, group_by, function, total_list, replace, page_breaks, summary_below_data) {#CellArea-int-ConsolidationFunction-list-bool-bool-bool}
Crea subtotales para el rango.



```python
def subtotal(self, ca, group_by, function, total_list, replace, page_breaks, summary_below_data):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| ca | [CellArea](/cells/es/python-net/aspose.cells/cellarea) | El rango|
| group_by | int | El campo por el que agrupar, como un desplazamiento de entero basado en cero|
| function | [ConsolidationFunction](/cells/es/python-net/aspose.cells/consolidationfunction) | La función de subtotales.|
| total_list | list | Una matriz de compensaciones de campo de base cero, que indica los campos a los que se agregan los subtotales.|
| replace | bool | Indica si se deben reemplazar los subtotales actuales|
| page_breaks | bool | Indica si agregar salto de página entre grupos|
| summary_below_data | bool | Indica si se agrega un resumen debajo de los datos.|



###  Ver también
* módulo [aspose.cells](../../)
* clase [Cells](/cells/es/python-net/aspose.cells/cells)
