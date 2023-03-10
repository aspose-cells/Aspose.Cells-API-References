---
title: ImageOrPrintOptions класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 40
url: /ru/python-net/aspose.cells.rendering/imageorprintoptions/
is_root: false
---
##  ImageOrPrintOptions класс
Позволяет указать параметры при рендеринге рабочего листа в изображения, печати рабочего листа или рендеринга диаграммы в изображение.



Тип ImageOrPrintOptions предоставляет следующие члены:

###  Конструкторы
| Конструктор| Описание|
| :- | :- |
| [ImageOrPrintOptions()](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/__init__/#) | Создает новый экземпляр ImageOrPrintOptions|


###  Характеристики
| Свойство| Описание|
| :- | :- |
| [save_format](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/save_format) | Получает или задает тип формата выходного файла<br/> Поддержка Tiff/XPS|
| [print_with_status_dialog](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/print_with_status_dialog) | Если PrintWithStatusDialog = true, появится диалоговое окно, показывающее текущее состояние печати.<br/> иначе такой диалог не будет отображаться.|
| [horizontal_resolution](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/horizontal_resolution) | Получает или задает разрешение по горизонтали для сгенерированных изображений в точках на дюйм.<br/> Применяет метод генерации изображения, за исключением изображений в формате EMF.|
| [vertical_resolution](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/vertical_resolution) | Получает или задает вертикальное разрешение для сгенерированных изображений в точках на дюйм.<br/> Применяет метод генерации изображения, за исключением изображения в формате Emf.|
| [tiff_compression](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/tiff_compression) | Получает или задает тип сжатия, применяемый только при сохранении страниц в формате `Tiff`.|
| [tiff_color_depth](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/tiff_color_depth) | Получает или задает разрядность, которая применяется только при сохранении страниц в формате `Tiff`.|
| [printing_page](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/printing_page) | Указывает, какие страницы не будут распечатаны.|
| [quality](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/quality) | Получает или задает значение, определяющее качество сгенерированных изображений.<br/>применять только при сохранении страниц в формате `Jpeg`. Значение по умолчанию – 100.|
| [image_type](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/image_type) | Получает или задает формат сгенерированных изображений.<br/> значение по умолчанию: PNG.|
| [is_cell_auto_fit](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/is_cell_auto_fit) | Указывает, подгоняются ли ширина и высота ячеек автоматически по значению ячейки.<br/> Значение по умолчанию неверно.|
| [one_page_per_sheet](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/one_page_per_sheet) | Если OnePagePerSheet имеет значение true , все содержимое одного листа будет выводиться только на одну страницу в результате.<br/> Размер бумаги в pagesetup будет неверным, а другие настройки pagesetup<br/> все равно вступит в силу.|
| [all_columns_in_one_page_per_sheet](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/all_columns_in_one_page_per_sheet) | Если AllColumnsInOnePagePerSheet имеет значение true , все содержимое столбцов одного листа будет выведено только на одну страницу в результате.<br/> Ширина размера бумаги в pagesetup будет недействительной, а другие настройки pagesetup<br/> все равно вступит в силу.|
| [draw_object_event_handler](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/draw_object_event_handler) | Реализует этот интерфейс для получения DrawObject и Bound при рендеринге.|
| [chart_image_type](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/chart_image_type) | Укажите тип изображения диаграммы при конвертации.<br/> значение по умолчанию: PNG.|
| [embeded_image_name_in_svg](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/embeded_image_name_in_svg) | Укажите имя файла встроенного изображения в svg.<br/> Это должен быть полный путь с каталогом типа "c:\\xpsEmbedded"|
| [svg_fit_to_view_port](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/svg_fit_to_view_port) | если это свойство истинно, сгенерированный svg будет соответствовать порту просмотра.|
| [only_area](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/only_area) | Если это свойство имеет значение true , будет выведена одна область, и масштаб не будет действовать.|
| [text_rendering_hint](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/text_rendering_hint) | Определяет качество рендеринга текста.<br/> Значение по умолчанию — TextRenderingHint.SystemDefault.|
| [smoothing_mode](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/smoothing_mode) | Указывает, применяется ли сглаживание (сглаживание) к линиям и кривым, а также к краям заполненных областей.<br/> Значение по умолчанию — SmoothingMode.None.|
| [transparent](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/transparent) | Указывает, должен ли фон сгенерированного изображения быть прозрачным.|
| [pixel_format](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/pixel_format) |Получает или задает формат пикселей для сгенерированных изображений.|
| [warning_callback](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/warning_callback) | Получает или задает обратный вызов предупреждения.|
| [page_saving_callback](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/page_saving_callback) | Управление/указание хода процесса сохранения страницы.|
| [is_font_substitution_char_granularity](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/is_font_substitution_char_granularity) | Указывает, следует ли заменять шрифт символа только в том случае, если шрифт ячейки несовместим с ним.|
| [page_index](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/page_index) | Получает или задает отсчитываемый от 0 индекс первой страницы для сохранения.|
| [page_count](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/page_count) | Получает или задает количество страниц для сохранения.|
| [is_optimized](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/is_optimized) | Указывает, следует ли оптимизировать элементы вывода.|
| [default_font](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/default_font) | Когда символы в Excel имеют формат Unicode и для них не задан правильный шрифт в стиле ячейки,<br/>Они могут отображаться как блок в pdf, изображение.<br/>Установите DefaultFont, например MingLiu или MS Gothic, чтобы отображались эти символы.<br/> Если это свойство не установлено, Aspose.Cells будет использовать системный шрифт по умолчанию для отображения этих символов Юникода.|
| [check_workbook_default_font](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/check_workbook_default_font) | Когда символы в Excel имеют формат Unicode и для них не задан правильный шрифт в стиле ячейки,<br/>Они могут отображаться как блок в pdf, изображение.<br/> Установите для этого параметра значение true, чтобы попытаться использовать шрифт рабочей книги по умолчанию для отображения этих символов в первую очередь.|
| [output_blank_page_when_nothing_to_print](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/output_blank_page_when_nothing_to_print) | Указывает, следует ли выводить пустую страницу, когда нечего печатать.|
| [gridline_type](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/gridline_type) | Получает или задает тип линии сетки.|
| [text_cross_type](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/text_cross_type) | Получает или задает отображаемый тип текста, когда ширина текста больше ширины ячейки.|
| [emf_type](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/emf_type) | Получает или задает EmfType, указывающий формат метафайла.<br/> Значение по умолчанию — EmfPlusDual.|
| [default_edit_language](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/default_edit_language) | Получает или задает язык редактирования по умолчанию.|
| [sheet_set](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/sheet_set) |Получает или задает листы для отображения. По умолчанию все видимые листы в книге: [SheetSet.visible](/cells/ru/python-net/aspose.cells.rendering/sheetset#visible).|


###  Методы
| Метод| Описание|
| :- | :- |
| [set_desired_size(desired_width, desired_height)](/cells/ru/python-net/aspose.cells.rendering/imageorprintoptions/set_desired_size/#int-int) | Устанавливает желаемую ширину и высоту изображения.|



###  Пример

```python
from aspose.cells import Workbook
from aspose.cells.drawing import ImageType
from aspose.cells.rendering import ImageOrPrintOptions

# Set Image Or Print Options
options = ImageOrPrintOptions()
# Set output image format
options.image_type = ImageType.PNG
# Set Horizontal resolution
options.horizontal_resolution = 300
# Set Vertical Resolution
options.vertical_resolution = 300
# Instantiate Workbook
book = Workbook("test.xls")
# Save chart as Image using ImageOrPrint Options
book.worksheets[0].charts[0].to_image("chart.png", options)

```

###  Смотрите также
* модуль [aspose.cells.rendering](..)
