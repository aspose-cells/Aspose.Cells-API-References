---
title: start_cell метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 40
url: /ru/python-net/aspose.cells/lightcellsdatahandler/start_cell/
is_root: false
---
##  start_cell(column_index) {#int}
Готовится к обработке ячейки.


###  Возвращает

нужно ли обрабатывать эту ячейку.false, чтобы игнорировать ячейку и проверять следующую, пока не будет достигнут конец данных ячеек текущей строки


```python
def start_cell(self, column_index):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| column_index | int | индекс столбца ячейки для обработки|
###  Примечания

Он будет вызываться при достижении существующей ячейки в текущей строке Текущая строка — это строка последнего вызова [LightCellsDataHandler.process_row(row)](/cells/ru/python-net/aspose.cells/lightcellsdatahandler/process_row).


###  Смотрите также

* модуль [aspose.cells](../../)
* класс [LightCellsDataHandler](/cells/ru/python-net/aspose.cells/lightcellsdatahandler)
