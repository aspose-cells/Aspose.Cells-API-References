---
title: add_filter método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 40
url: /es/python-net/aspose.cells/autofilter/add_filter/
is_root: false
---
##  add_filter(field_index, criteria) {#int-str}
Agrega un filtro para una columna de filtro.



```python
def add_filter(self, field_index, criteria):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| field_index | int | El desplazamiento entero del campo en el que desea basar el filtro<br/> (desde la izquierda de la lista; el campo más a la izquierda es el campo 0).|
| criteria | str | Los criterios especificados (una cadena; por ejemplo, "101").<br/> Solo puede ser nulo o ser uno de los valores de las celdas en esta columna.|
###  Observaciones

MS Excel 2007 admite la selección múltiple en una columna de filtro.


###  Ver también

* módulo [aspose.cells](../../)
* clase [AutoFilter](/cells/es/python-net/aspose.cells/autofilter)
