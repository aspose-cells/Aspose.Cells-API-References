---
title: start_sheet метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 70
url: /ru/python-net/aspose.cells/lightcellsdataprovider/start_sheet/
is_root: false
---
##  start_sheet(sheet_index) {#int}
Начинает сохранять рабочий лист.


###  Возвращает

true, если этот провайдер предоставит данные для данного листа; false, если данный лист должен использовать свою обычную модель данных (Cells).


```python
def start_sheet(self, sheet_index):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| sheet_index | int | индекс текущего листа для сохранения.|
###  Примечания

Он будет вызываться в начале сохранения листа во время сохранения книги.
 Если провайдеру необходимо обратиться к*`индекс листа`* позже
в методе startRow(Row) или startCell(Cell),
 то есть, если процессу необходимо знать, какой рабочий лист обрабатывается,
 реализация должна сохранить*`индекс листа`* значение здесь.


###  Смотрите также
* модуль [aspose.cells](../../)
* класс [LightCellsDataProvider](/cells/ru/python-net/aspose.cells/lightcellsdataprovider)
