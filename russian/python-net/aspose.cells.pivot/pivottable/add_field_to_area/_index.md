---
title: add_field_to_area метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 30
url: /ru/python-net/aspose.cells.pivot/pivottable/add_field_to_area/
is_root: false
---
##  add_field_to_area(field_type, field_name) {#PivotFieldType-str}
Добавляет поле в определенную область.


###  Возвращает

Позиция поля в определенных полях. Если поля с таким именем нет, вернуть -1.


```python
def add_field_to_area(self, field_type, field_name):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| field_type | [PivotFieldType](/cells/ru/python-net/aspose.cells.pivot/pivotfieldtype) | Тип области поля.|
| field_name | str | Имя в базовых полях.|


##  add_field_to_area(field_type, base_field_index) {#PivotFieldType-int}
Добавляет поле в определенную область.


###  Возвращает

Позиция поля в определенных полях.


```python
def add_field_to_area(self, field_type, base_field_index):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| field_type | [PivotFieldType](/cells/ru/python-net/aspose.cells.pivot/pivotfieldtype) | Тип области поля.|
| base_field_index | int | Индекс поля в базовых полях.|


##  add_field_to_area(field_type, pivot_field) {#PivotFieldType-PivotField}
Добавляет поле в определенную область.


###  Возвращает

положение поля в конкретных полях.


```python
def add_field_to_area(self, field_type, pivot_field):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| field_type | [PivotFieldType](/cells/ru/python-net/aspose.cells.pivot/pivotfieldtype) | тип области поля.|
| pivot_field | [PivotField](/cells/ru/python-net/aspose.cells.pivot/pivotfield) | поле в базовых полях.|



###  Смотрите также
* модуль [aspose.cells.pivot](../../)
* класс [PivotTable](/cells/ru/python-net/aspose.cells.pivot/pivottable)
