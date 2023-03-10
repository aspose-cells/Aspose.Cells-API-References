---
title: metodo add_date_filter
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 20
url: /it/python-net/aspose.cells/autofilter/add_date_filter/
is_root: false
---
##  add_date_filter(field_index, date_time_grouping_type, year, month, day, hour, minute, second) {#int-DateTimeGroupingType-int-int-int-int-int-int}
Aggiunge un filtro data.



```python
def add_date_filter(self, field_index, date_time_grouping_type, year, month, day, hour, minute, second):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| field_index | int | L'intero offset del campo su cui si desidera basare il filtro<br/> (da sinistra dell'elenco; il campo più a sinistra è il campo 0).|
| date_time_grouping_type | [DateTimeGroupingType](/cells/it/python-net/aspose.cells/datetimegroupingtype) | [DateTimeGroupingType](/cells/it/python-net/aspose.cells/datetimegroupingtype) |
| year | int | L'anno.|
| month | int | Il mese.|
| day | int | Il giorno.|
| hour | int | L'ora.|
| minute | int | Il minuto.|
| second | int | Il secondo.|
###  Osservazioni

Se DateTimeGroupingType è Year, ha effetto solo il parametro year.
Se DateTiemGroupingType è Month, ha effetto solo il parametro anno e mese.


###  Guarda anche
* modulo [aspose.cells](../../)
* classe [AutoFilter](/cells/it/python-net/aspose.cells/autofilter)
* classe [DateTimeGroupingType](/cells/it/python-net/aspose.cells/datetimegroupingtype)
