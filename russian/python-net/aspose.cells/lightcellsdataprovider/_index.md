---
title: LightCellsDataProvider класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 1000
url: /ru/python-net/aspose.cells/lightcellsdataprovider/
is_root: false
---
##  LightCellsDataProvider класс
Представляет поставщика данных для сохранения больших файлов электронных таблиц в облегченном режиме.



Тип LightCellsDataProvider предоставляет следующие члены:

###  Методы
| Метод| Описание|
| :- | :- |
| [start_sheet(sheet_index)](/cells/ru/python-net/aspose.cells/lightcellsdataprovider/start_sheet/#int) | Начинает сохранять рабочий лист.|
| [next_row()](/cells/ru/python-net/aspose.cells/lightcellsdataprovider/next_row/#) | Получает следующую строку для сохранения.|
| [start_row(row)](/cells/ru/python-net/aspose.cells/lightcellsdataprovider/start_row/#Row) | Начинает сохранять данные одной строки.|
| [next_cell()](/cells/ru/python-net/aspose.cells/lightcellsdataprovider/next_cell/#) | Получает следующую ячейку для сохранения.|
| [start_cell(cell)](/cells/ru/python-net/aspose.cells/lightcellsdataprovider/start_cell/#Cell) | Начинает сохранять данные одной ячейки.|
| [is_gather_string()](/cells/ru/python-net/aspose.cells/lightcellsdataprovider/is_gather_string/#) |Проверяет, нужно ли собирать текущее строковое значение ячейки в глобальный пул.|



###  Примечания

При сохранении книги в этом режиме [LightCellsDataProvider.start_sheet(sheet_index)](/cells/ru/python-net/aspose.cells/lightcellsdataprovider/start_sheet) будет проверяться при сохранении каждого листа в книге.
Для одного листа, если [LightCellsDataProvider.start_sheet(sheet_index)](/cells/ru/python-net/aspose.cells/lightcellsdataprovider/start_sheet) дает true, то сохраняются все данные и свойства строк/ячеек этого листа
будет обеспечен реализацией этого интерфейса.Во-первых, [LightCellsDataProvider.next_row()](/cells/ru/python-net/aspose.cells/lightcellsdataprovider/next_row) будет вызываться для получения следующего индекса строки для сохранения.
Если возвращается допустимый индекс строки (индекс строки должен быть в порядке возрастания для сохранения строк),
затем объект Row, представляющий эту строку, будет предоставлен для реализации, чтобы установить ее свойства по [LightCellsDataProvider.start_row(row)](/cells/ru/python-net/aspose.cells/lightcellsdataprovider/start_row).
Для одной строки сначала будет проверено [LightCellsDataProvider.next_cell()](/cells/ru/python-net/aspose.cells/lightcellsdataprovider/next_cell). Если будет возвращен допустимый индекс столбца (индекс столбца должен быть в порядке возрастания для сохранения всех ячеек одной строки),
затем объект Cell, представляющий эту ячейку, будет предоставлен для реализации, чтобы установить ее данные и свойства по [LightCellsDataProvider.start_cell(cell)](/cells/ru/python-net/aspose.cells/lightcellsdataprovider/start_cell).
После того, как данные этой ячейки будут установлены, эта ячейка будет сохранена непосредственно в сгенерированном файле электронной таблицы, а следующая ячейка будет проверена и обработана.

###  Смотрите также
* модуль [aspose.cells](..)
