---
title: get_style_in_pool метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 190
url: /ru/python-net/aspose.cells/workbook/get_style_in_pool/
is_root: false
---
##  get_style_in_pool(index) {#int}
Получает стиль из пула стилей.
Все стили в книге будут собраны в пул.
В ячейках есть только простой ссылочный индекс.


###  Возвращает

Стиль в пуле соответствует заданному индексу, может быть нулевым.


```python
def get_style_in_pool(self, index):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| index | int | Индекс.|
###  Примечания

Если возвращенный стиль изменен, стиль всех ячеек (которые относятся к этому стилю) будут изменены.


###  Смотрите также

* модуль [aspose.cells](../../)
* класс [Workbook](/cells/ru/python-net/aspose.cells/workbook)
