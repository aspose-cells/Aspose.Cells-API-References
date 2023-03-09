---
title: remove_date_filter метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 150
url: /ru/python-net/aspose.cells/autofilter/remove_date_filter/
is_root: false
---
##  remove_date_filter(field_index, date_time_grouping_type, year, month, day, hour, minute, second) {#int-DateTimeGroupingType-int-int-int-int-int-int}
Удаляет фильтр даты.



```python
def remove_date_filter(self, field_index, date_time_grouping_type, year, month, day, hour, minute, second):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| field_index | int | Целочисленное смещение поля, на котором вы хотите основывать фильтр.<br/> (слева в списке; крайнее левое поле — поле 0).|
| date_time_grouping_type | [DateTimeGroupingType](/cells/ru/python-net/aspose.cells/datetimegroupingtype) | [DateTimeGroupingType](/cells/ru/python-net/aspose.cells/datetimegroupingtype) |
| year | int | Год.|
| month | int | Месяц.|
| day | int | День.|
| hour | int | Час.|
| minute | int | Минута.|
| second | int | Второй.|
###  Примечания

Если DateTimeGroupingType имеет значение Year, действует только параметр year.
Если DateTiemGroupingType имеет значение Month, действуют только параметры года и месяца.


###  Смотрите также
* модуль [aspose.cells](../../)
* класс [AutoFilter](/cells/ru/python-net/aspose.cells/autofilter)
* класс [DateTimeGroupingType](/cells/ru/python-net/aspose.cells/datetimegroupingtype)
