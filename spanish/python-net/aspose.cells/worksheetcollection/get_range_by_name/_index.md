---
title: get_range_by_name método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 120
url: /es/python-net/aspose.cells/worksheetcollection/get_range_by_name/
is_root: false
---
##  get_range_by_name(range_name) {#str}
Obtiene el objeto Range por nombre predefinido.


###  Devoluciones

Objeto de rango.


Devuelve nulo si el rango con nombre no existe.


```python
def get_range_by_name(self, range_name):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| range_name | str | Nombre del rango.|


##  get_range_by_name(range_name, current_sheet_index, include_table) {#str-int-bool}
Obtiene [Range](/cells/es/python-net/aspose.cells/range) por nombre predefinido o nombre de tabla


###  Devoluciones




```python
def get_range_by_name(self, range_name, current_sheet_index, include_table):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| range_name | str | Nombre del rango o nombre de la tabla.|
| current_sheet_index | int | El índice de la hoja. -1 representa global.|
| include_table | bool | Indica si se revisan todas las tablas.|



###  Ver también
* módulo [aspose.cells](../../)
* clase [Range](/cells/es/python-net/aspose.cells/range)
* clase [WorksheetCollection](/cells/es/python-net/aspose.cells/worksheetcollection)
