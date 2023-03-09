---
title: set_manual_group_field метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 210
url: /ru/python-net/aspose.cells.pivot/pivottable/set_manual_group_field/
is_root: false
---
##  set_manual_group_field(base_field_index, start_val, end_val, group_by_list, interval_num) {#int-float-float-list-float}
Задает группу полей вручную для сводной таблицы.



```python
def set_manual_group_field(self, base_field_index, start_val, end_val, group_by_list, interval_num):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| base_field_index | int | Индекс поля строки или столбца в базовых полях|
| start_val | float |Задает начальное значение для числовой группировки.|
| end_val | float | Указывает конечное значение для числовой группировки.|
| group_by_list | list | Задает список типов группировки. Задается PivotTableGroupType|
| interval_num | float | Указывает группу номеров интервалов по числовой группировке.|


##  set_manual_group_field(pivot_field, start_val, end_val, group_by_list, interval_num) {#PivotField-float-float-list-float}
Задает группу полей вручную для сводной таблицы.



```python
def set_manual_group_field(self, pivot_field, start_val, end_val, group_by_list, interval_num):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| pivot_field | [PivotField](/cells/ru/python-net/aspose.cells.pivot/pivotfield) | Поле строки или столбца в базовых полях|
| start_val | float |Задает начальное значение для числовой группировки.|
| end_val | float | Указывает конечное значение для числовой группировки.|
| group_by_list | list | Задает список типов группировки. Задается PivotTableGroupType|
| interval_num | float | Указывает группу номеров интервалов по числовой группировке.|


##  set_manual_group_field(base_field_index, start_val, end_val, group_by_list, interval_num) {#int-DateTime-DateTime-list-int}
Задает группу полей вручную для сводной таблицы.



```python
def set_manual_group_field(self, base_field_index, start_val, end_val, group_by_list, interval_num):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| base_field_index | int | Индекс поля строки или столбца в базовых полях|
| start_val | DateTime | Задает начальное значение для группировки дат.|
| end_val | DateTime | Задает конечное значение для группировки дат.|
| group_by_list | list | Задает список типов группировки. Задается PivotTableGroupType|
| interval_num | int | Указывает группу номеров интервалов по дням группировки. Количество дней должно быть положительным целым числом, отличным от нуля.|


##  set_manual_group_field(pivot_field, start_val, end_val, group_by_list, interval_num) {#PivotField-DateTime-DateTime-list-int}
Задает группу полей вручную для сводной таблицы.



```python
def set_manual_group_field(self, pivot_field, start_val, end_val, group_by_list, interval_num):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| pivot_field | [PivotField](/cells/ru/python-net/aspose.cells.pivot/pivotfield) | Поле строки или столбца в базовых полях|
| start_val | DateTime | Задает начальное значение для группировки дат.|
| end_val | DateTime | Задает конечное значение для группировки дат.|
| group_by_list | list | Задает список типов группировки. Задается PivotTableGroupType|
| interval_num | int | Указывает группу номеров интервалов по дням группировки. Количество дней должно быть положительным целым числом, отличным от нуля.|



###  Смотрите также
* модуль [aspose.cells.pivot](../../)
* класс [PivotTable](/cells/ru/python-net/aspose.cells.pivot/pivottable)
