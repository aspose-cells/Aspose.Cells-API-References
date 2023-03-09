---
title: add_identify método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 20
url: /es/python-net/aspose.cells.pivot/pivotpagefields/add_identify/
is_root: false
---
##  add_identify(range_index, page_item_index) {#int-list}
Establece qué etiqueta de elemento en cada campo de página usar para identificar el rango de datos.
El pageItemIndex.Length debe ser igual a PageFieldCount, así que agregue el campo de la página primero.



```python
def add_identify(self, range_index, page_item_index):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| range_index | int | El índice de rango de datos de consolidación.|
| page_item_index | list | El índice de elementos de página en cada campo de página.<br/>pageItemIndex[2] = 1 significa el segundo elemento en el tercer campo que se usará para identificar este rango.<br/> pageItemIndex[1] = -1 significa que no hay elemento en el segundo campo para usar para identificar este rango<br/> y MS creará automáticamente un elemento "en blanco" en el segundo campo para identificar este rango.|



###  Ver también
* módulo [aspose.cells.pivot](../../)
* clase [PivotPageFields](/cells/es/python-net/aspose.cells.pivot/pivotpagefields)
