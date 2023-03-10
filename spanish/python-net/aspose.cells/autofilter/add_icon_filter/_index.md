---
title: add_icon_filter método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 60
url: /es/python-net/aspose.cells/autofilter/add_icon_filter/
is_root: false
---
##  add_icon_filter(field_index, icon_set_type, icon_id) {#int-IconSetType-int}
Añade un filtro de iconos.



```python
def add_icon_filter(self, field_index, icon_set_type, icon_id):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| field_index | int | El desplazamiento entero del campo en el que desea basar el filtro<br/> (desde la izquierda de la lista; el campo más a la izquierda es el campo 0).|
| icon_set_type | [IconSetType](/cells/es/python-net/aspose.cells/iconsettype) | El tipo de conjunto de iconos.|
| icon_id | int | La identificación del icono.|
###  Observaciones

Solo admite agregar el filtro de iconos.
No admite verificar qué fila está visible si el filtro es un filtro de íconos.


###  Ver también
* módulo [aspose.cells](../../)
* clase [AutoFilter](/cells/es/python-net/aspose.cells/autofilter)
