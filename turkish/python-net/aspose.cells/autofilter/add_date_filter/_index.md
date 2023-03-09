---
title: add_date_filter yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 20
url: /tr/python-net/aspose.cells/autofilter/add_date_filter/
is_root: false
---
##  add_date_filter(field_index, date_time_grouping_type, year, month, day, hour, minute, second) {#int-DateTimeGroupingType-int-int-int-int-int-int}
Bir tarih filtresi ekler.



```python
def add_date_filter(self, field_index, date_time_grouping_type, year, month, day, hour, minute, second):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| field_index | int | Filtreyi temel almak istediğiniz alanın tamsayı ofseti<br/> (listenin solundan; en soldaki alan 0 alanıdır).|
| date_time_grouping_type | [DateTimeGroupingType](/cells/tr/python-net/aspose.cells/datetimegroupingtype) | [DateTimeGroupingType](/cells/tr/python-net/aspose.cells/datetimegroupingtype) |
| year | int | Yıl.|
| month | int | Ay.|
| day | int | Gün.|
| hour | int | Saat.|
| minute | int | Dakika.|
| second | int | İkinci.|
###  Notlar

DateTimeGroupingType Yıl ise, yalnızca param yıl etkileri.
DateTiemGroupingType Ay ise, yalnızca parametre yıl ve ay etkisi.


###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [AutoFilter](/cells/tr/python-net/aspose.cells/autofilter)
* sınıf [DateTimeGroupingType](/cells/tr/python-net/aspose.cells/datetimegroupingtype)
