---
title: add_date_filter metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 20
url: /sv/python-net/aspose.cells/autofilter/add_date_filter/
is_root: false
---
##  add_date_filter(field_index, date_time_grouping_type, year, month, day, hour, minute, second) {#int-DateTimeGroupingType-int-int-int-int-int-int}
Lägger till ett datumfilter.



```python
def add_date_filter(self, field_index, date_time_grouping_type, year, month, day, hour, minute, second):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| field_index | int | Heltalsoffset för fältet som du vill basera filtret på<br/> (från vänster i listan; fältet längst till vänster är fält 0).|
| date_time_grouping_type | [DateTimeGroupingType](/cells/sv/python-net/aspose.cells/datetimegroupingtype) | [DateTimeGroupingType](/cells/sv/python-net/aspose.cells/datetimegroupingtype) |
| year | int | Året.|
| month | int | Månaden.|
| day | int | Dagen.|
| hour | int | Timmen.|
| minute | int | Minuten.|
| second | int | Den andra.|
###  Anmärkningar

Om DateTimeGroupingType är Year, påverkar endast paramåret.
Om DateTiemGroupingType är Month, gäller endast param år och månad.


###  Se även
* modul [aspose.cells](../../)
* klass [AutoFilter](/cells/sv/python-net/aspose.cells/autofilter)
* klass [DateTimeGroupingType](/cells/sv/python-net/aspose.cells/datetimegroupingtype)
