---
title: PdfSaveOptions класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 1180
url: /ru/python-net/aspose.cells/pdfsaveoptions/
is_root: false
---
##  PdfSaveOptions класс
Представляет параметры для сохранения файла PDF.



**Наследование:** [PdfSaveOptions](/cells/python-net/aspose.cells/pdfsaveoptions) → 
[PaginatedSaveOptions](/cells/python-net/aspose.cells/paginatedsaveoptions) → 
[SaveOptions](/cells/ru/python-net/aspose.cells/saveoptions)



Тип PdfSaveOptions предоставляет следующие члены:

###  Конструкторы
| Конструктор| Описание|
| :- | :- |
| [PdfSaveOptions()](/cells/ru/python-net/aspose.cells/pdfsaveoptions/__init__/#) | Создает параметры для сохранения файла PDF.|


###  Характеристики
| Свойство| Описание|
| :- | :- |
| [save_format](/cells/ru/python-net/aspose.cells/pdfsaveoptions/save_format) | Получает формат файла сохранения.|
| [clear_data](/cells/ru/python-net/aspose.cells/pdfsaveoptions/clear_data) | Сделайте рабочую книгу пустой после сохранения файла.|
| [cached_file_folder](/cells/ru/python-net/aspose.cells/pdfsaveoptions/cached_file_folder) | Папка с кэшированными файлами используется для хранения больших данных.|
| [validate_merged_areas](/cells/ru/python-net/aspose.cells/pdfsaveoptions/validate_merged_areas) | Указывает, следует ли проверять объединенные ячейки перед сохранением файла.|
| [merge_areas](/cells/ru/python-net/aspose.cells/pdfsaveoptions/merge_areas) | Указывает, объединяются ли области условного форматирования и проверки перед сохранением файла.|
| [create_directory](/cells/ru/python-net/aspose.cells/pdfsaveoptions/create_directory) | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла.|
| [sort_names](/cells/ru/python-net/aspose.cells/pdfsaveoptions/sort_names) | Указывает, выполняется ли сортировка определенных имен перед сохранением файла.|
| [sort_external_names](/cells/ru/python-net/aspose.cells/pdfsaveoptions/sort_external_names) | Указывает, выполняется ли сортировка внешних определенных имен перед сохранением файла.|
| [refresh_chart_cache](/cells/ru/python-net/aspose.cells/pdfsaveoptions/refresh_chart_cache) |Указывает, обновляются ли данные кэша диаграммы.|
| [warning_callback](/cells/ru/python-net/aspose.cells/pdfsaveoptions/warning_callback) | Получает или задает обратный вызов предупреждения.|
| [update_smart_art](/cells/ru/python-net/aspose.cells/pdfsaveoptions/update_smart_art) | Указывает, обновляются ли настройки смарт-арта.<br/> Значение по умолчанию неверно.|
| [default_font](/cells/ru/python-net/aspose.cells/pdfsaveoptions/default_font) | Когда символы в Excel имеют формат Unicode и для них не задан правильный шрифт в стиле ячейки,<br/>Они могут отображаться как блок в pdf, изображение.<br/>Установите DefaultFont, например MingLiu или MS Gothic, чтобы отображались эти символы.<br/> Если это свойство не установлено, Aspose.Cells будет использовать системный шрифт по умолчанию для отображения этих символов Юникода.|
| [check_workbook_default_font](/cells/ru/python-net/aspose.cells/pdfsaveoptions/check_workbook_default_font) | Когда символы в Excel имеют формат Unicode и для них не задан правильный шрифт в стиле ячейки,<br/>Они могут отображаться как блок в pdf, изображение.<br/> Установите для этого параметра значение true, чтобы попытаться использовать шрифт рабочей книги по умолчанию для отображения этих символов в первую очередь.|
| [check_font_compatibility](/cells/ru/python-net/aspose.cells/pdfsaveoptions/check_font_compatibility) | Указывает, следует ли проверять совместимость шрифтов для каждого символа в тексте.|
| [is_font_substitution_char_granularity](/cells/ru/python-net/aspose.cells/pdfsaveoptions/is_font_substitution_char_granularity) | Указывает, следует ли заменять шрифт символа только в том случае, если шрифт ячейки несовместим с ним.|
| [one_page_per_sheet](/cells/ru/python-net/aspose.cells/pdfsaveoptions/one_page_per_sheet) | Если OnePagePerSheet имеет значение true , все содержимое одного листа будет выводиться только на одну страницу в результате.<br/> Размер бумаги в pagesetup будет неверным, а другие настройки pagesetup<br/> все равно вступит в силу.|
| [all_columns_in_one_page_per_sheet](/cells/ru/python-net/aspose.cells/pdfsaveoptions/all_columns_in_one_page_per_sheet) | Если AllColumnsInOnePagePerSheet имеет значение true , все содержимое столбцов одного листа будет выведено только на одну страницу в результате.<br/> Ширина размера бумаги pagesetup будет игнорироваться, а другие настройки pagesetup<br/> все равно вступит в силу.|
| [ignore_error](/cells/ru/python-net/aspose.cells/pdfsaveoptions/ignore_error) | Указывает, нужно ли скрыть ошибку при рендеринге.<br/> Ошибка может быть ошибкой в форме, изображении, рендеринге диаграммы и т. д.|
| [output_blank_page_when_nothing_to_print](/cells/ru/python-net/aspose.cells/pdfsaveoptions/output_blank_page_when_nothing_to_print) | Указывает, следует ли выводить пустую страницу, когда нечего печатать.|
| [page_index](/cells/ru/python-net/aspose.cells/pdfsaveoptions/page_index) | Получает или задает отсчитываемый от 0 индекс первой страницы для сохранения.|
| [page_count](/cells/ru/python-net/aspose.cells/pdfsaveoptions/page_count) | Получает или задает количество страниц для сохранения.|
| [printing_page_type](/cells/ru/python-net/aspose.cells/pdfsaveoptions/printing_page_type) | Указывает, какие страницы не будут распечатаны.|
| [gridline_type](/cells/ru/python-net/aspose.cells/pdfsaveoptions/gridline_type) | Получает или задает тип линии сетки.|
| [text_cross_type](/cells/ru/python-net/aspose.cells/pdfsaveoptions/text_cross_type) | Получает или задает отображаемый тип текста, когда ширина текста больше ширины ячейки.|
| [default_edit_language](/cells/ru/python-net/aspose.cells/pdfsaveoptions/default_edit_language) | Получает или задает язык редактирования по умолчанию.|
| [sheet_set](/cells/ru/python-net/aspose.cells/pdfsaveoptions/sheet_set) |Получает или задает листы для отображения. По умолчанию все видимые листы в книге: [SheetSet.visible](/cells/ru/python-net/aspose.cells.rendering/sheetset#visible).|
| [draw_object_event_handler](/cells/ru/python-net/aspose.cells/pdfsaveoptions/draw_object_event_handler) | Реализует этот интерфейс для получения DrawObject и Bound при рендеринге.|
| [page_saving_callback](/cells/ru/python-net/aspose.cells/pdfsaveoptions/page_saving_callback) |Управление/указание хода процесса сохранения страницы.|
| [embed_standard_windows_fonts](/cells/ru/python-net/aspose.cells/pdfsaveoptions/embed_standard_windows_fonts) | Значение true для встраивания шрифтов истинного типа.<br/>Влияет только на символы ASCII 32-127.<br/>Шрифты для кодов символов больше 127 всегда встроены.<br/>Шрифты всегда встроены для стандарта PDF/A-1a, PDF/A-1b.<br/> Значение по умолчанию верно.|
| [bookmark](/cells/ru/python-net/aspose.cells/pdfsaveoptions/bookmark) | Получает и задает объект [PdfBookmarkEntry](/cells/ru/python-net/aspose.cells.rendering/pdfbookmarkentry).|
| [compliance](/cells/ru/python-net/aspose.cells/pdfsaveoptions/compliance) | Рабочая книга преобразуется в pdf в соответствии с PdfCompliance в этом свойстве.|
| [security_options](/cells/ru/python-net/aspose.cells/pdfsaveoptions/security_options) | Установите эти параметры, когда требуется безопасность в результате xls2pdf.|
| [image_type](/cells/ru/python-net/aspose.cells/pdfsaveoptions/image_type) | Представляет тип изображения при преобразовании диаграммы и фигуры.|
| [calculate_formula](/cells/ru/python-net/aspose.cells/pdfsaveoptions/calculate_formula) | Указывает, следует ли вычислять формулы перед сохранением файла PDF.|
| [pdf_compression](/cells/ru/python-net/aspose.cells/pdfsaveoptions/pdf_compression) |Укажите алгоритм сжатия|
| [created_time](/cells/ru/python-net/aspose.cells/pdfsaveoptions/created_time) | Получает и задает время создания pdf-документа.|
| [producer](/cells/ru/python-net/aspose.cells/pdfsaveoptions/producer) | Получает и устанавливает производителя сгенерированного PDF-документа.|
| [optimization_type](/cells/ru/python-net/aspose.cells/pdfsaveoptions/optimization_type) | Получает и устанавливает тип оптимизации PDF.|
| [custom_properties_export](/cells/ru/python-net/aspose.cells/pdfsaveoptions/custom_properties_export) | Получает или задает значение, определяющее способ экспорта [CustomDocumentPropertyCollection](/cells/ru/python-net/aspose.cells.properties/customdocumentpropertycollection) в файл PDF. Значение по умолчанию — Нет.|
| [export_document_structure](/cells/ru/python-net/aspose.cells/pdfsaveoptions/export_document_structure) | Указывает, следует ли экспортировать структуру документа.|
| [emf_render_setting](/cells/ru/python-net/aspose.cells/pdfsaveoptions/emf_render_setting) | Настройка для рендеринга метафайла EMF.|
| [display_doc_title](/cells/ru/python-net/aspose.cells/pdfsaveoptions/display_doc_title) | Указывает, должна ли строка заголовка окна отображать заголовок документа.|
| [font_encoding](/cells/ru/python-net/aspose.cells/pdfsaveoptions/font_encoding) | Получает или задает встроенную кодировку шрифта в pdf.|


###  Методы
| Метод| Описание|
| :- | :- |
| [set_image_resample(desired_ppi, jpeg_quality)](/cells/ru/python-net/aspose.cells/pdfsaveoptions/set_image_resample/#int-int) | Устанавливает желаемое значение PPI (пикселей на дюйм) изображений с повторной выборкой и качество JPEG.<br/> Все изображения будут преобразованы в формат JPEG с указанной настройкой качества,<br/>и изображения, которые превышают указанный PPI (пикселей на дюйм), будут передискретизированы.|



###  Смотрите также
* модуль [aspose.cells](..)
* класс [CustomDocumentPropertyCollection](/cells/ru/python-net/aspose.cells.properties/customdocumentpropertycollection)
* класс [PaginatedSaveOptions](/cells/ru/python-net/aspose.cells/paginatedsaveoptions)
* класс [PdfBookmarkEntry](/cells/ru/python-net/aspose.cells.rendering/pdfbookmarkentry)
* класс [PdfSaveOptions](/cells/ru/python-net/aspose.cells/pdfsaveoptions)
* класс [SaveOptions](/cells/ru/python-net/aspose.cells/saveoptions)
