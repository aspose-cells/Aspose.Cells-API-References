---
title: HtmlSaveOptions класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 780
url: /ru/python-net/aspose.cells/htmlsaveoptions/
is_root: false
---
##  HtmlSaveOptions класс
Представляет параметры для сохранения html-файла.



**Наследование:** [HtmlSaveOptions](/cells/python-net/aspose.cells/htmlsaveoptions) → 
[SaveOptions](/cells/ru/python-net/aspose.cells/saveoptions)



Тип HtmlSaveOptions предоставляет следующие члены:

###  Конструкторы
| Конструктор| Описание|
| :- | :- |
| [HtmlSaveOptions()](/cells/ru/python-net/aspose.cells/htmlsaveoptions/__init__/#) | Создает параметры для сохранения html-файла.|
| [HtmlSaveOptions(format)](/cells/ru/python-net/aspose.cells/htmlsaveoptions/__init__/#SaveFormat) | Создает параметры для сохранения файла htm.|


###  Характеристики
| Свойство| Описание|
| :- | :- |
| [save_format](/cells/ru/python-net/aspose.cells/htmlsaveoptions/save_format) | Получает формат файла сохранения.|
| [clear_data](/cells/ru/python-net/aspose.cells/htmlsaveoptions/clear_data) | Сделайте рабочую книгу пустой после сохранения файла.|
| [cached_file_folder](/cells/ru/python-net/aspose.cells/htmlsaveoptions/cached_file_folder) | Папка с кэшированными файлами используется для хранения больших данных.|
| [validate_merged_areas](/cells/ru/python-net/aspose.cells/htmlsaveoptions/validate_merged_areas) | Указывает, следует ли проверять объединенные ячейки перед сохранением файла.|
| [merge_areas](/cells/ru/python-net/aspose.cells/htmlsaveoptions/merge_areas) | Указывает, объединяются ли области условного форматирования и проверки перед сохранением файла.|
| [create_directory](/cells/ru/python-net/aspose.cells/htmlsaveoptions/create_directory) | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла.|
| [sort_names](/cells/ru/python-net/aspose.cells/htmlsaveoptions/sort_names) | Указывает, выполняется ли сортировка определенных имен перед сохранением файла.|
| [sort_external_names](/cells/ru/python-net/aspose.cells/htmlsaveoptions/sort_external_names) |Указывает, выполняется ли сортировка внешних определенных имен перед сохранением файла.|
| [refresh_chart_cache](/cells/ru/python-net/aspose.cells/htmlsaveoptions/refresh_chart_cache) | Указывает, обновляются ли данные кэша диаграммы.|
| [warning_callback](/cells/ru/python-net/aspose.cells/htmlsaveoptions/warning_callback) | Получает или задает обратный вызов предупреждения.|
| [update_smart_art](/cells/ru/python-net/aspose.cells/htmlsaveoptions/update_smart_art) | Указывает, обновляются ли настройки смарт-арта.<br/> Значение по умолчанию неверно.|
| [ignore_invisible_shapes](/cells/ru/python-net/aspose.cells/htmlsaveoptions/ignore_invisible_shapes) |Укажите, экспортируются ли невидимые фигуры|
| [page_title](/cells/ru/python-net/aspose.cells/htmlsaveoptions/page_title) | Заголовок html-страницы.<br/> Только для сохранения в html поток.|
| [attached_files_directory](/cells/ru/python-net/aspose.cells/htmlsaveoptions/attached_files_directory) | Каталог, в который будут сохранены вложенные файлы.<br/> Только для сохранения в html поток.|
| [attached_files_url_prefix](/cells/ru/python-net/aspose.cells/htmlsaveoptions/attached_files_url_prefix) | Укажите префикс URL вложенных файлов, таких как изображение в файле html.<br/> Только для сохранения в html поток.|
| [default_font_name](/cells/ru/python-net/aspose.cells/htmlsaveoptions/default_font_name) | Укажите имя шрифта по умолчанию для экспорта html, шрифт по умолчанию будет использоваться, если шрифт стиля не существует,<br/>Если это свойство равно null, Aspose.Cells будет использовать универсальный шрифт, имеющий то же семейство, что и исходный шрифт.<br/> значение по умолчанию равно нулю.|
| [worksheet_scalable](/cells/ru/python-net/aspose.cells/htmlsaveoptions/worksheet_scalable) | Указывает, что при увеличении или уменьшении масштаба html с помощью уровня масштабирования листа при сохранении файла в html значение по умолчанию равно false.|
| [is_export_comments](/cells/ru/python-net/aspose.cells/htmlsaveoptions/is_export_comments) | Указывает, что при экспорте комментариев при сохранении файла в формате html значение по умолчанию равно false.|
| [export_comments_type](/cells/ru/python-net/aspose.cells/htmlsaveoptions/export_comments_type) | Представляет тип экспорта комментариев в файлы html.|
| [disable_downlevel_revealed_comments](/cells/ru/python-net/aspose.cells/htmlsaveoptions/disable_downlevel_revealed_comments) | Указывает, что при отключении условных комментариев, отображаемых на нижнем уровне, при экспорте файла в html значение по умолчанию равно false.|
| [is_exp_image_to_temp_dir](/cells/ru/python-net/aspose.cells/htmlsaveoptions/is_exp_image_to_temp_dir) | Указывает, экспортируются ли файлы изображений во временный каталог.<br/> Только для сохранения в html поток.|
| [image_scalable](/cells/ru/python-net/aspose.cells/htmlsaveoptions/image_scalable) | Указывает, используется ли масштабируемая единица для описания ширины изображения.<br/>при использовании масштабируемой единицы для описания ширины столбца.<br/> Значение по умолчанию верно.|
| [width_scalable](/cells/ru/python-net/aspose.cells/htmlsaveoptions/width_scalable) |Указывает, используются ли масштабируемые единицы для описания ширины столбца при экспорте файла в html.<br/> Значение по умолчанию неверно.|
| [export_single_tab](/cells/ru/python-net/aspose.cells/htmlsaveoptions/export_single_tab) | Указывает, следует ли экспортировать одну вкладку, если файл содержит только один рабочий лист.<br/> Значение по умолчанию неверно.|
| [export_images_as_base64](/cells/ru/python-net/aspose.cells/htmlsaveoptions/export_images_as_base64) | Указывает, сохраняются ли изображения в формате Base64 в HTML, MHTML или EPUB.|
| [export_active_worksheet_only](/cells/ru/python-net/aspose.cells/htmlsaveoptions/export_active_worksheet_only) | Указывает, экспортируется ли вся книга в html-файл.|
| [export_print_area_only](/cells/ru/python-net/aspose.cells/htmlsaveoptions/export_print_area_only) | Указывает, экспортируется ли только область печати в html-файл. Значение по умолчанию неверно.|
| [export_area](/cells/ru/python-net/aspose.cells/htmlsaveoptions/export_area) | Получает или задает экспортируемую CellArea текущего активного рабочего листа.<br/>Если вы установите этот атрибут, область печати текущего активного рабочего листа будет опущена.<br/> При сохранении файла в html будет экспортирована только указанная область.|
| [parse_html_tag_in_cell](/cells/ru/python-net/aspose.cells/htmlsaveoptions/parse_html_tag_in_cell) | Разобрать HTML-тег в ячейке, например, как значение ячейки или как HTML-тег, по умолчанию — true|
| [html_cross_string_type](/cells/ru/python-net/aspose.cells/htmlsaveoptions/html_cross_string_type) | Указывает, будет ли строка между ячейками отображаться так же, как в MS Excel, при сохранении файла Excel в формате html.<br/>По умолчанию используется значение «По умолчанию», поэтому для строк между ячейками разница между html-файлами, созданными Aspose.Cells, и MS Excel незначительна.<br/> Но производительность при создании больших html-файлов при установке значения Cross будет в несколько раз выше, чем при установке значения Default или Fit2Cell.|
| [hidden_col_display_type](/cells/ru/python-net/aspose.cells/htmlsaveoptions/hidden_col_display_type) |Скрытый столбец (ширина этого столбца равна 0) в excel, прежде чем сохранить его в формате html,<br/>если HtmlHiddenColDisplayType имеет значение «Удалить», скрытый столбец не будет выводиться,<br/> если значение «Скрытый», столбец будет выводиться, но будет скрыт, значение по умолчанию — «Скрытый».|
| [hidden_row_display_type](/cells/ru/python-net/aspose.cells/htmlsaveoptions/hidden_row_display_type) | Скрытая строка (высота этой строки равна 0) в excel, перед сохранением в формате html,<br/>если HtmlHiddenRowDisplayType имеет значение «Удалить», скрытая строка не будет выводиться,<br/> если значение «Скрыто», строка будет выводиться, но будет скрыта, значение по умолчанию — «Скрыто».|
| [encoding](/cells/ru/python-net/aspose.cells/htmlsaveoptions/encoding) | Если не задано, используйте Encoding.UTF8 в качестве типа кодировки по умолчанию.|
| [export_object_listener](/cells/ru/python-net/aspose.cells/htmlsaveoptions/export_object_listener) | Получает или задает ExportObjectListener для экспорта объектов.|
| [file_path_provider](/cells/ru/python-net/aspose.cells/htmlsaveoptions/file_path_provider) | Получает или задает IFilePathProvider для отдельного экспорта рабочего листа в HTML.|
| [stream_provider](/cells/ru/python-net/aspose.cells/htmlsaveoptions/stream_provider) | Получает или задает IStreamProvider для экспорта объектов.|
| [image_options](/cells/ru/python-net/aspose.cells/htmlsaveoptions/image_options) | Получите объект ImageOrPrintOptions перед экспортом|
| [save_as_single_file](/cells/ru/python-net/aspose.cells/htmlsaveoptions/save_as_single_file) | Указывает, следует ли сохранять html как один файл.<br/> Значение по умолчанию неверно.|
| [show_all_sheets](/cells/ru/python-net/aspose.cells/htmlsaveoptions/show_all_sheets) | Указывает, будут ли отображаться все листы при сохранении в виде одного HTML-файла.|
| [export_page_headers](/cells/ru/python-net/aspose.cells/htmlsaveoptions/export_page_headers) | Указывает, экспортируются ли заголовки страниц.|
| [export_page_footers](/cells/ru/python-net/aspose.cells/htmlsaveoptions/export_page_footers) | Указывает, экспортируются ли заголовки страниц.|
| [export_hidden_worksheet](/cells/ru/python-net/aspose.cells/htmlsaveoptions/export_hidden_worksheet) |Указывает, экспортируется ли скрытое содержимое рабочего листа. Значение по умолчанию — true.|
| [presentation_preference](/cells/ru/python-net/aspose.cells/htmlsaveoptions/presentation_preference) | Указание, является ли файл html или mht предпочтительным для представления.<br/>Значение по умолчанию неверно.<br/> если вы хотите получить более красивую презентацию, установите значение true.|
| [cell_css_prefix](/cells/ru/python-net/aspose.cells/htmlsaveoptions/cell_css_prefix) | Получает и устанавливает префикс имени css, значение по умолчанию — «».|
| [table_css_id](/cells/ru/python-net/aspose.cells/htmlsaveoptions/table_css_id) | Получает и устанавливает префикс имени типа css, например, tr,col,td и т. д., они содержатся в элементе таблицы<br/> который имеет определенный атрибут TableCssId. Значение по умолчанию — «».|
| [is_full_path_link](/cells/ru/python-net/aspose.cells/htmlsaveoptions/is_full_path_link) | Указывает, используется ли ссылка полного пути в sheet00x.htm, filelist.xml и tabstrip.htm.<br/> Значение по умолчанию неверно.|
| [export_worksheet_css_separately](/cells/ru/python-net/aspose.cells/htmlsaveoptions/export_worksheet_css_separately) | Указывает, экспортировать ли рабочий лист css отдельно. Значение по умолчанию — false.|
| [export_similar_border_style](/cells/ru/python-net/aspose.cells/htmlsaveoptions/export_similar_border_style) | Указывает, экспортируется ли аналогичный стиль границы, если стиль границы не поддерживается браузерами.<br/>Если вы хотите импортировать файл html или mht в Excel, оставьте значение по умолчанию.<br/> Значение по умолчанию неверно.|
| [merge_empty_td_forcely](/cells/ru/python-net/aspose.cells/htmlsaveoptions/merge_empty_td_forcely) | Указывает, будет ли принудительно объединяться пустой элемент TD при экспорте файла в html.<br/> Размер html-файла будет значительно уменьшен после установки значения true. Значение по умолчанию неверно.<br/> Если вы хотите импортировать html-файл в Excel или экспортировать идеальные линии сетки при сохранении файла в html,<br/> пожалуйста, оставьте значение по умолчанию.|
| [export_cell_coordinate](/cells/ru/python-net/aspose.cells/htmlsaveoptions/export_cell_coordinate) |Указывает, экспортируются ли координаты excel непустых ячеек при сохранении файла в html. Значение по умолчанию неверно.<br/> Если вы хотите импортировать выходной HTML-код в Excel, оставьте значение по умолчанию.|
| [export_extra_headings](/cells/ru/python-net/aspose.cells/htmlsaveoptions/export_extra_headings) | Указывает, экспортируются ли дополнительные заголовки, когда длина текста превышает максимальную отображаемую колонку.<br/> Значение по умолчанию неверно. Если вы хотите импортировать html-файл в Excel, оставьте значение по умолчанию.|
| [export_headings](/cells/ru/python-net/aspose.cells/htmlsaveoptions/export_headings) | Указывает, экспортируются ли заголовки строк и столбцов листа при сохранении в файлы HTML.|
| [export_row_column_headings](/cells/ru/python-net/aspose.cells/htmlsaveoptions/export_row_column_headings) | Указывает, экспортируются ли заголовки строк и столбцов листа при сохранении в файлы HTML.|
| [export_formula](/cells/ru/python-net/aspose.cells/htmlsaveoptions/export_formula) | Указывает, будет ли экспортироваться формула при сохранении файла в html. Значение по умолчанию верно.<br/> Если вы хотите импортировать выходной HTML-код в Excel, оставьте значение по умолчанию.|
| [add_tooltip_text](/cells/ru/python-net/aspose.cells/htmlsaveoptions/add_tooltip_text) | Указывает, следует ли добавлять текст всплывающей подсказки, когда данные не могут быть полностью отображены.<br/> Значение по умолчанию неверно.|
| [export_grid_lines](/cells/ru/python-net/aspose.cells/htmlsaveoptions/export_grid_lines) | Указывает, экспортируются ли линии сетки. Значение по умолчанию — false.|
| [export_bogus_row_data](/cells/ru/python-net/aspose.cells/htmlsaveoptions/export_bogus_row_data) | Указывает, экспортируются ли фиктивные данные нижней строки. Значение по умолчанию — true. Если вы хотите импортировать файл html или mht<br/> чтобы преуспеть, оставьте значение по умолчанию.|
| [exclude_unused_styles](/cells/ru/python-net/aspose.cells/htmlsaveoptions/exclude_unused_styles) | Указывает, исключает ли неиспользуемые стили.<br/>Для сгенерированных html-файлов исключение неиспользуемых стилей может уменьшить размер файла.<br/>без ущерба для визуальных эффектов. Таким образом, значение этого свойства по умолчанию равно true.<br/>Если пользователю необходимо сохранить все стили в рабочей книге для сгенерированного html (например, сценарий, в котором пользователь<br/>необходимо восстановить книгу из сгенерированного html позже), установите для этого свойства значение false.|
| [export_document_properties](/cells/ru/python-net/aspose.cells/htmlsaveoptions/export_document_properties) | Указывает, экспортируются ли свойства документа. Значение по умолчанию — true. Если вы хотите импортировать<br/> файл html или mht, чтобы преуспеть, оставьте значение по умолчанию.|
| [export_worksheet_properties](/cells/ru/python-net/aspose.cells/htmlsaveoptions/export_worksheet_properties) | Указывает, экспортируются ли свойства рабочего листа. Значение по умолчанию — true. Если вы хотите импортировать<br/> файл html или mht, чтобы преуспеть, оставьте значение по умолчанию.|
| [export_workbook_properties](/cells/ru/python-net/aspose.cells/htmlsaveoptions/export_workbook_properties) | Указывает, экспортируются ли свойства книги. Значение по умолчанию — true. Если вы хотите импортировать<br/> файл html или mht, чтобы преуспеть, оставьте значение по умолчанию.|
| [export_frame_scripts_and_properties](/cells/ru/python-net/aspose.cells/htmlsaveoptions/export_frame_scripts_and_properties) | Указание, следует ли экспортировать сценарии фреймов и свойства документа. Значение по умолчанию — true. Если вы хотите импортировать файл html или mht<br/> чтобы преуспеть, оставьте значение по умолчанию.|
| [export_data_options](/cells/ru/python-net/aspose.cells/htmlsaveoptions/export_data_options) | Указание правила экспорта данных файла html. Значение по умолчанию — All.|
| [link_target_type](/cells/ru/python-net/aspose.cells/htmlsaveoptions/link_target_type) | Указание типа целевого атрибута в<a> ссылка, значение по умолчанию — HtmlLinkTargetType.Parent.|



###  Смотрите также
* модуль [aspose.cells](..)
* класс [HtmlSaveOptions](/cells/ru/python-net/aspose.cells/htmlsaveoptions)
* класс [SaveOptions](/cells/ru/python-net/aspose.cells/saveoptions)
