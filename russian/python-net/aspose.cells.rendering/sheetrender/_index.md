---
title: SheetRender класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 100
url: /ru/python-net/aspose.cells.rendering/sheetrender/
is_root: false
---
##  SheetRender класс
Представляет визуализацию рабочего листа, который может отображать рабочий лист для различных изображений, таких как (BMP, PNG, JPEG, TIFF..)
Конструктор этого класса должен использоваться после модификации pagesetup, стиля ячейки.



Тип SheetRender предоставляет следующие члены:

###  Конструкторы
| Конструктор| Описание|
| :- | :- |
| [SheetRender(worksheet, options)](/cells/ru/python-net/aspose.cells.rendering/sheetrender/__init__/#Worksheet-ImageOrPrintOptions) | конструкция SheetRender, нужен рабочий лист и ImageOrPrintOptions в качестве параметров|


###  Характеристики
| Свойство| Описание|
| :- | :- |
| [page_count](/cells/ru/python-net/aspose.cells.rendering/sheetrender/page_count) | Получает общее количество страниц текущего рабочего листа.|
| [page_scale](/cells/ru/python-net/aspose.cells.rendering/sheetrender/page_scale) | Получает рассчитанный масштаб страницы листа.<br/> Возвращает заданный масштаб, если установлено значение [PageSetup.zoom](/cells/ru/python-net/aspose.cells/pagesetup#zoom).|


###  Методы
| Метод| Описание|
| :- | :- |
| [to_image(page_index, file_name)](/cells/ru/python-net/aspose.cells.rendering/sheetrender/to_image/#int-str) | Рендеринг определенных страниц в файл.|
| [to_image(page_index, stream)](/cells/ru/python-net/aspose.cells.rendering/sheetrender/to_image/#int-io.RawIOBase) | Рендеринг определенных страниц в поток.|
| [to_tiff(stream)](/cells/ru/python-net/aspose.cells.rendering/sheetrender/to_tiff/#io.RawIOBase) | Визуализируйте весь рабочий лист в виде изображения Tiff для потоковой передачи.|
| [to_tiff(filename)](/cells/ru/python-net/aspose.cells.rendering/sheetrender/to_tiff/#str) | Визуализация всего рабочего листа в виде изображения Tiff в файл.|
| [to_printer(printer_name)](/cells/ru/python-net/aspose.cells.rendering/sheetrender/to_printer/#str) | Вывод рабочего листа на принтер|
| [to_printer(printer_name, job_name)](/cells/ru/python-net/aspose.cells.rendering/sheetrender/to_printer/#str-str) | Вывод рабочего листа на принтер|
| [to_printer(printer_settings)](/cells/ru/python-net/aspose.cells.rendering/sheetrender/to_printer/#aspose.pydrawing.printing.PrinterSettings) | Вывод рабочего листа на принтер|
| [to_printer(printer_settings, job_name)](/cells/ru/python-net/aspose.cells.rendering/sheetrender/to_printer/#aspose.pydrawing.printing.PrinterSettings-str) | Вывод рабочего листа на принтер|
| [to_printer(printer_name, print_page_index, print_page_count)](/cells/ru/python-net/aspose.cells.rendering/sheetrender/to_printer/#str-int-int) | Вывод рабочего листа на принтер|
| [get_page_size_inch(page_index)](/cells/ru/python-net/aspose.cells.rendering/sheetrender/get_page_size_inch/#int) |Получить размер страницы в дюймах выходного изображения.|
| [custom_print(next_page_after_print, print_page_event_args)](/cells/ru/python-net/aspose.cells.rendering/sheetrender/custom_print/#bool-aspose.pydrawing.printing.PrintPageEventArgs) | Клиент может управлять настройками страницы принтера при печати каждой страницы с помощью этой функции.|



###  Смотрите также
* модуль [aspose.cells.rendering](..)
