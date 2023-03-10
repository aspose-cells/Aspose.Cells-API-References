---
title: to_printer метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 50
url: /ru/python-net/aspose.cells.rendering/workbookrender/to_printer/
is_root: false
---
##  to_printer(printer_name) {#str}
Рендеринг книги на принтер



```python
def to_printer(self, printer_name):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| printer_name | str | имя принтера, например: "Microsoft Office Document Image Writer"|


##  to_printer(printer_settings) {#aspose.pydrawing.printing.PrinterSettings}
Рендеринг книги на принтер



```python
def to_printer(self, printer_settings):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| printer_settings | aspose.pydrawing.printing.PrinterSettings | настройки принтера, например PrinterName, Duplex|


##  to_printer(printer_name, job_name) {#str-str}
Рендеринг книги на принтер



```python
def to_printer(self, printer_name, job_name):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| printer_name | str | имя принтера, например: "Microsoft Office Document Image Writer"|
| job_name | str | установить имя задания на печать|


##  to_printer(printer_settings, job_name) {#aspose.pydrawing.printing.PrinterSettings-str}
Рендеринг книги на принтер



```python
def to_printer(self, printer_settings, job_name):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| printer_settings | aspose.pydrawing.printing.PrinterSettings | настройки принтера, например PrinterName, Duplex|
| job_name | str | установить имя задания на печать|


##  to_printer(printer_name, print_page_index, print_page_count) {#str-int-int}
Рендеринг книги на принтер



```python
def to_printer(self, printer_name, print_page_index, print_page_count):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| printer_name | str | имя принтера, например: "Microsoft Office Document Image Writer"|
| print_page_index | int | основанный на 0 индекс первой страницы для печати, он должен быть в диапазоне [0, WorkbookRender.PageCount-1]|
| print_page_count | int | количество страниц для печати, оно должно быть больше нуля|
###  Примечания

ПРИМЕЧАНИЕ. Этот метод устарел.
Вместо этого используйте ToPrinter(string PrinterName) и ImageOrPrintOptions.PageIndex, PageCount, чтобы установить первую страницу и количество страниц для печати.
 Это свойство будет удалено через 12 месяцев, начиная с декабря 2021 года.
Aspose приносит извинения за возможные неудобства.


###  Смотрите также
* модуль [aspose.cells.rendering](../../)
* класс [WorkbookRender](/cells/ru/python-net/aspose.cells.rendering/workbookrender)
