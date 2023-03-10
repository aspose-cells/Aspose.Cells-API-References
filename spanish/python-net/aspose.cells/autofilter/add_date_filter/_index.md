---
title: add_date_filter método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 20
url: /es/python-net/aspose.cells/autofilter/add_date_filter/
is_root: false
---
##  add_date_filter(field_index, date_time_grouping_type, year, month, day, hour, minute, second) {#int-DateTimeGroupingType-int-int-int-int-int-int}
Agrega un filtro de fecha.



```python
def add_date_filter(self, field_index, date_time_grouping_type, year, month, day, hour, minute, second):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| field_index | int | El desplazamiento entero del campo en el que desea basar el filtro<br/> (desde la izquierda de la lista; el campo más a la izquierda es el campo 0).|
| date_time_grouping_type | [DateTimeGroupingType](/cells/es/python-net/aspose.cells/datetimegroupingtype) | [DateTimeGroupingType](/cells/es/python-net/aspose.cells/datetimegroupingtype) |
| year | int | El año.|
| month | int | El mes.|
| day | int | El dia.|
| hour | int | La hora.|
| minute | int | El minuto.|
| second | int | El segundo.|
###  Observaciones

Si DateTimeGroupingType es Year, solo se aplica el parámetro year.
Si DateTiemGroupingType es Mes, solo el parámetro año y mes tienen efecto.


###  Ver también
* módulo [aspose.cells](../../)
* clase [AutoFilter](/cells/es/python-net/aspose.cells/autofilter)
* clase [DateTimeGroupingType](/cells/es/python-net/aspose.cells/datetimegroupingtype)
