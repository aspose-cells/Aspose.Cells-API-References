---
title: index_of метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 40
url: /ru/python-net/aspose.cells.properties/documentpropertycollection/index_of/
is_root: false
---
##  index_of(name) {#str}
Получает индекс свойства по имени.


###  Возвращает

Индекс, основанный на нуле. Отрицательное значение, если не найдено.


```python
def index_of(self, name):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| name | str | Нечувствительное к регистру имя свойства.|


##  index_of(item, index) {#DocumentProperty-int}
Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который простирается от указанного индекса до последнего элемента.


###  Возвращает

Отсчитываемый от нуля индекс первого вхождения значения в диапазоне элементов в списке массивов, который простирается от startIndex до последнего элемента, если он найден; в противном случае -1.


```python
def index_of(self, item, index):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| item | [DocumentProperty](/cells/ru/python-net/aspose.cells.properties/documentproperty) | Объект, который нужно найти в списке массивов.|
| index | int | Начальный индекс поиска, отсчитываемый от нуля. 0 (ноль) допустим в пустом списке.|


##  index_of(item, index, count) {#DocumentProperty-int-int}
Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который начинается с указанного индекса и содержит указанное количество элементов.


###  Возвращает

Отсчитываемый от нуля индекс первого вхождения значения в диапазоне элементов в списке массивов, который начинается с startIndex и содержит подсчитанное количество элементов, если он найден; в противном случае -1.


```python
def index_of(self, item, index, count):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| item | [DocumentProperty](/cells/ru/python-net/aspose.cells.properties/documentproperty) | Объект, который нужно найти в списке массивов.|
| index | int | Начальный индекс поиска, отсчитываемый от нуля. 0 (ноль) допустим в пустом списке.|
| count | int | Количество элементов в разделе для поиска.|



###  Смотрите также
* модуль [aspose.cells.properties](../../)
* класс [DocumentPropertyCollection](/cells/ru/python-net/aspose.cells.properties/documentpropertycollection)
