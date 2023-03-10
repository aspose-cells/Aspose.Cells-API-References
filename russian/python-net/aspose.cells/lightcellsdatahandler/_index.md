---
title: LightCellsDataHandler класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 990
url: /ru/python-net/aspose.cells/lightcellsdatahandler/
is_root: false
---
##  LightCellsDataHandler класс
Представляет обработчик данных ячеек для чтения больших файлов электронных таблиц в облегченном режиме.



Тип LightCellsDataHandler предоставляет следующие члены:

###  Методы
| Метод| Описание|
| :- | :- |
| [start_sheet(sheet)](/cells/ru/python-net/aspose.cells/lightcellsdatahandler/start_sheet/#Worksheet) | Начинает обрабатывать рабочий лист.|
| [start_row(row_index)](/cells/ru/python-net/aspose.cells/lightcellsdatahandler/start_row/#int) | Готовится к обработке строки.|
| [process_row(row)](/cells/ru/python-net/aspose.cells/lightcellsdatahandler/process_row/#Row) | Начинает обрабатывать одну строку.|
| [start_cell(column_index)](/cells/ru/python-net/aspose.cells/lightcellsdatahandler/start_cell/#int) | Готовится к обработке ячейки.|
| [process_cell(cell)](/cells/ru/python-net/aspose.cells/lightcellsdatahandler/process_cell/#Cell) | Начинает обрабатывать одну ячейку.|



###  Примечания

При чтении книги в этом режиме [LightCellsDataHandler.start_sheet(sheet)](/cells/ru/python-net/aspose.cells/lightcellsdatahandler/start_sheet) будет проверяться при чтении каждого листа в книге.
Для одного листа, если [LightCellsDataHandler.start_sheet(sheet)](/cells/ru/python-net/aspose.cells/lightcellsdatahandler/start_sheet) дает true, то будут проверены все данные и свойства строк/ячеек этого листа
и обрабатывается реализацией этого интерфейса. Для каждой строки будет вызываться [LightCellsDataHandler.start_row(row_index)](/cells/ru/python-net/aspose.cells/lightcellsdatahandler/start_row), чтобы проверить, нужно ли ее обрабатывать.
Если строку необходимо обработать, свойства этой строки будут считаны в первую очередь, и пользователь сможет получить доступ к ее свойствам по номеру [LightCellsDataHandler.process_row(row)](/cells/ru/python-net/aspose.cells/lightcellsdatahandler/process_row).
если ячейки строки также необходимо обработать, то [LightCellsDataHandler.process_row(row)](/cells/ru/python-net/aspose.cells/lightcellsdatahandler/process_row) должно вернуть true, а затем [LightCellsDataHandler.start_cell(column_index)](/cells/ru/python-net/aspose.cells/lightcellsdatahandler/start_cell) будет
вызывается для каждой существующей ячейки в этой строке, чтобы проверить, нужно ли обрабатывать одну ячейку. Если нужно обработать одну ячейку,
затем будет вызван [LightCellsDataHandler.process_cell(cell)](/cells/ru/python-net/aspose.cells/lightcellsdatahandler/process_cell) для обработки ячейки реализацией этого интерфейса.

###  Смотрите также
* модуль [aspose.cells](..)
