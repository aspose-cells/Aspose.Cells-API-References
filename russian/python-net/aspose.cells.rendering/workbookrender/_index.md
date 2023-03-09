---
title: WorkbookRender класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 130
url: /ru/python-net/aspose.cells.rendering/workbookrender/
is_root: false
---
##  WorkbookRender класс
 Представляет визуализацию рабочей книги.
Конструктор этого класса должен использоваться после модификации pagesetup, стиля ячейки.



Тип WorkbookRender предоставляет следующие члены:

###  Конструкторы
| Конструктор| Описание|
| :- | :- |
| [WorkbookRender(workbook, options)](/cells/ru/python-net/aspose.cells.rendering/workbookrender/__init__/#Workbook-ImageOrPrintOptions) | Конструкция WorkbookRender|


###  Характеристики
| Свойство| Описание|
| :- | :- |
| [page_count](/cells/ru/python-net/aspose.cells.rendering/workbookrender/page_count) | Получает общее количество страниц книг.|


###  Методы
| Метод| Описание|
| :- | :- |
| [to_image(stream)](/cells/ru/python-net/aspose.cells.rendering/workbookrender/to_image/#io.RawIOBase) | Рендеринг всей книги в виде изображения Tiff для потоковой передачи.|
| [to_image(filename)](/cells/ru/python-net/aspose.cells.rendering/workbookrender/to_image/#str) | Визуализация всей книги в виде изображения Tiff в файл.|
| [to_image(page_index, file_name)](/cells/ru/python-net/aspose.cells.rendering/workbookrender/to_image/#int-str) | Рендеринг определенных страниц в файл.|
| [to_image(page_index, stream)](/cells/ru/python-net/aspose.cells.rendering/workbookrender/to_image/#int-io.RawIOBase) | Рендеринг определенных страниц в поток.|
| [to_printer(printer_name)](/cells/ru/python-net/aspose.cells.rendering/workbookrender/to_printer/#str) | Вывод книги на принтер|
| [to_printer(printer_name, job_name)](/cells/ru/python-net/aspose.cells.rendering/workbookrender/to_printer/#str-str) | Вывод книги на принтер|
| [to_printer(printer_settings)](/cells/ru/python-net/aspose.cells.rendering/workbookrender/to_printer/#aspose.pydrawing.printing.PrinterSettings) | Вывод книги на принтер|
| [to_printer(printer_settings, job_name)](/cells/ru/python-net/aspose.cells.rendering/workbookrender/to_printer/#aspose.pydrawing.printing.PrinterSettings-str) | Вывод книги на принтер|
| [to_printer(printer_name, print_page_index, print_page_count)](/cells/ru/python-net/aspose.cells.rendering/workbookrender/to_printer/#str-int-int) | Вывод книги на принтер|
| [get_page_size_inch(page_index)](/cells/ru/python-net/aspose.cells.rendering/workbookrender/get_page_size_inch/#int) |Получить размер страницы в дюймах выходного изображения.|
| [custom_print(next_page_after_print, print_page_event_args)](/cells/ru/python-net/aspose.cells.rendering/workbookrender/custom_print/#bool-aspose.pydrawing.printing.PrintPageEventArgs) | Клиент может управлять настройками страницы принтера при печати каждой страницы с помощью этой функции.|



###  Примечания



###  Смотрите также
* модуль [aspose.cells.rendering](..)
