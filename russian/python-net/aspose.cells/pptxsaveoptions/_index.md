---
title: PptxSaveOptions класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 1190
url: /ru/python-net/aspose.cells/pptxsaveoptions/
is_root: false
---
##  PptxSaveOptions класс
Представляет параметры сохранения pptx.



**Наследование:** [PptxSaveOptions](/cells/python-net/aspose.cells/pptxsaveoptions) → 
[PaginatedSaveOptions](/cells/python-net/aspose.cells/paginatedsaveoptions) → 
[SaveOptions](/cells/ru/python-net/aspose.cells/saveoptions)



Тип PptxSaveOptions предоставляет следующие члены:

###  Конструкторы
| Конструктор| Описание|
| :- | :- |
| [PptxSaveOptions()](/cells/ru/python-net/aspose.cells/pptxsaveoptions/__init__/#) | Представляет параметры сохранения pptx.|
| [PptxSaveOptions(save_as_image)](/cells/ru/python-net/aspose.cells/pptxsaveoptions/__init__/#bool) | Представляет варианты сохранения файла .pptx.|


###  Характеристики
| Свойство| Описание|
| :- | :- |
| [save_format](/cells/ru/python-net/aspose.cells/pptxsaveoptions/save_format) | Получает формат файла сохранения.|
| [clear_data](/cells/ru/python-net/aspose.cells/pptxsaveoptions/clear_data) | Сделайте рабочую книгу пустой после сохранения файла.|
| [cached_file_folder](/cells/ru/python-net/aspose.cells/pptxsaveoptions/cached_file_folder) | Папка с кэшированными файлами используется для хранения больших данных.|
| [validate_merged_areas](/cells/ru/python-net/aspose.cells/pptxsaveoptions/validate_merged_areas) | Указывает, следует ли проверять объединенные ячейки перед сохранением файла.|
| [merge_areas](/cells/ru/python-net/aspose.cells/pptxsaveoptions/merge_areas) | Указывает, объединяются ли области условного форматирования и проверки перед сохранением файла.|
| [create_directory](/cells/ru/python-net/aspose.cells/pptxsaveoptions/create_directory) | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла.|
| [sort_names](/cells/ru/python-net/aspose.cells/pptxsaveoptions/sort_names) | Указывает, выполняется ли сортировка определенных имен перед сохранением файла.|
| [sort_external_names](/cells/ru/python-net/aspose.cells/pptxsaveoptions/sort_external_names) |Указывает, выполняется ли сортировка внешних определенных имен перед сохранением файла.|
| [refresh_chart_cache](/cells/ru/python-net/aspose.cells/pptxsaveoptions/refresh_chart_cache) | Указывает, обновляются ли данные кэша диаграммы.|
| [warning_callback](/cells/ru/python-net/aspose.cells/pptxsaveoptions/warning_callback) | Получает или задает обратный вызов предупреждения.|
| [update_smart_art](/cells/ru/python-net/aspose.cells/pptxsaveoptions/update_smart_art) | Указывает, обновляются ли настройки смарт-арта.<br/> Значение по умолчанию неверно.|
| [default_font](/cells/ru/python-net/aspose.cells/pptxsaveoptions/default_font) | Когда символы в Excel имеют формат Unicode и для них не задан правильный шрифт в стиле ячейки,<br/>Они могут отображаться как блок в pdf, изображение.<br/>Установите DefaultFont, например MingLiu или MS Gothic, чтобы отображались эти символы.<br/> Если это свойство не установлено, Aspose.Cells будет использовать системный шрифт по умолчанию для отображения этих символов Юникода.|
| [check_workbook_default_font](/cells/ru/python-net/aspose.cells/pptxsaveoptions/check_workbook_default_font) | Когда символы в Excel имеют формат Unicode и для них не задан правильный шрифт в стиле ячейки,<br/>Они могут отображаться как блок в pdf, изображение.<br/> Установите для этого параметра значение true, чтобы попытаться использовать шрифт рабочей книги по умолчанию для отображения этих символов в первую очередь.|
| [check_font_compatibility](/cells/ru/python-net/aspose.cells/pptxsaveoptions/check_font_compatibility) |Указывает, следует ли проверять совместимость шрифтов для каждого символа в тексте.|
| [is_font_substitution_char_granularity](/cells/ru/python-net/aspose.cells/pptxsaveoptions/is_font_substitution_char_granularity) | Указывает, следует ли заменять шрифт символа только в том случае, если шрифт ячейки несовместим с ним.|
| [one_page_per_sheet](/cells/ru/python-net/aspose.cells/pptxsaveoptions/one_page_per_sheet) | Если OnePagePerSheet имеет значение true , все содержимое одного листа будет выводиться только на одну страницу в результате.<br/> Размер бумаги в pagesetup будет неверным, а другие настройки pagesetup<br/> все равно вступит в силу.|
| [all_columns_in_one_page_per_sheet](/cells/ru/python-net/aspose.cells/pptxsaveoptions/all_columns_in_one_page_per_sheet) | Если AllColumnsInOnePagePerSheet имеет значение true , все содержимое столбцов одного листа будет выведено только на одну страницу в результате.<br/> Ширина размера бумаги pagesetup будет игнорироваться, а другие настройки pagesetup<br/> все равно вступит в силу.|
| [ignore_error](/cells/ru/python-net/aspose.cells/pptxsaveoptions/ignore_error) | Указывает, нужно ли скрыть ошибку при рендеринге.<br/> Ошибка может быть ошибкой в форме, изображении, рендеринге диаграммы и т. д.|
| [output_blank_page_when_nothing_to_print](/cells/ru/python-net/aspose.cells/pptxsaveoptions/output_blank_page_when_nothing_to_print) | Указывает, следует ли выводить пустую страницу, когда нечего печатать.|
| [page_index](/cells/ru/python-net/aspose.cells/pptxsaveoptions/page_index) | Получает или задает отсчитываемый от 0 индекс первой страницы для сохранения.|
| [page_count](/cells/ru/python-net/aspose.cells/pptxsaveoptions/page_count) | Получает или задает количество страниц для сохранения.|
| [printing_page_type](/cells/ru/python-net/aspose.cells/pptxsaveoptions/printing_page_type) | Указывает, какие страницы не будут распечатаны.|
| [gridline_type](/cells/ru/python-net/aspose.cells/pptxsaveoptions/gridline_type) | Получает или задает тип линии сетки.|
| [text_cross_type](/cells/ru/python-net/aspose.cells/pptxsaveoptions/text_cross_type) | Получает или задает отображаемый тип текста, когда ширина текста больше ширины ячейки.|
| [default_edit_language](/cells/ru/python-net/aspose.cells/pptxsaveoptions/default_edit_language) | Получает или задает язык редактирования по умолчанию.|
| [sheet_set](/cells/ru/python-net/aspose.cells/pptxsaveoptions/sheet_set) |Получает или задает листы для отображения. По умолчанию все видимые листы в книге: [SheetSet.visible](/cells/ru/python-net/aspose.cells.rendering/sheetset#visible).|
| [draw_object_event_handler](/cells/ru/python-net/aspose.cells/pptxsaveoptions/draw_object_event_handler) | Реализует этот интерфейс для получения DrawObject и Bound при рендеринге.|
| [page_saving_callback](/cells/ru/python-net/aspose.cells/pptxsaveoptions/page_saving_callback) | Управление/указание хода процесса сохранения страницы.|



###  Смотрите также
* модуль [aspose.cells](..)
* класс [PaginatedSaveOptions](/cells/ru/python-net/aspose.cells/paginatedsaveoptions)
* класс [PptxSaveOptions](/cells/ru/python-net/aspose.cells/pptxsaveoptions)
* класс [SaveOptions](/cells/ru/python-net/aspose.cells/saveoptions)
