---
title: PivotTable класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 100
url: /ru/python-net/aspose.cells.pivot/pivottable/
is_root: false
---
##  PivotTable класс
Краткое описание для PivotTable.



Тип PivotTable предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [is_excel_2003_compatible](/cells/ru/python-net/aspose.cells.pivot/pivottable/is_excel_2003_compatible) | Указывает, совместима ли сводная таблица с Excel2003 при обновлении сводной таблицы,<br/>если true, строка должна быть меньше или равна 255 символам, поэтому, если строка больше 255 символов,<br/>он будет усечен. если false, строка не будет иметь вышеупомянутого ограничения.<br/> Значение по умолчанию верно.|
| [refreshed_by_who](/cells/ru/python-net/aspose.cells.pivot/pivottable/refreshed_by_who) | Получает имя пользователя, который последний раз обновлял сводную таблицу.|
| [refresh_date](/cells/ru/python-net/aspose.cells.pivot/pivottable/refresh_date) | Получает дату последнего обновления сводной таблицы.|
| [pivot_table_style_name](/cells/ru/python-net/aspose.cells.pivot/pivottable/pivot_table_style_name) |Получает и задает имя стиля сводной таблицы.|
| [pivot_table_style_type](/cells/ru/python-net/aspose.cells.pivot/pivottable/pivot_table_style_type) | Получает и задает встроенный стиль сводной таблицы.|
| [column_fields](/cells/ru/python-net/aspose.cells.pivot/pivottable/column_fields) | Возвращает объект PivotFields, который в данный момент отображается как поля столбца.|
| [row_fields](/cells/ru/python-net/aspose.cells.pivot/pivottable/row_fields) |Возвращает объект PivotFields, который в данный момент отображается как поля строк.|
| [page_fields](/cells/ru/python-net/aspose.cells.pivot/pivottable/page_fields) | Возвращает объект PivotFields, который в данный момент отображается как поля страницы.|
| [data_fields](/cells/ru/python-net/aspose.cells.pivot/pivottable/data_fields) | Получает объект PivotField, представляющий все поля данных в сводной таблице.<br/>Только для чтения. Это будет инициализироваться только при наличии двух или более полей данных в DataPiovtFiels.<br/> Он используется только для добавления DataPivotField в область строк/столбцов сводной таблицы. По умолчанию находится в области строк.|
| [data_field](/cells/ru/python-net/aspose.cells.pivot/pivottable/data_field) | Получает объект PivotField, представляющий все поля данных в сводной таблице.<br/>Только для чтения. Это будет инициализироваться только при наличии двух или более полей данных в DataPiovtFiels.<br/> Он используется только для добавления DataPivotField в область строк/столбцов сводной таблицы. По умолчанию находится в области строк.|
| [base_fields](/cells/ru/python-net/aspose.cells.pivot/pivottable/base_fields) | Возвращает объект PivotFields, включающий все поля отчета сводной таблицы.|
| [pivot_filters](/cells/ru/python-net/aspose.cells.pivot/pivottable/pivot_filters) | Возвращает объект PivotFilterCollection.|
| [column_range](/cells/ru/python-net/aspose.cells.pivot/pivottable/column_range) | Возвращает объект CellArea, представляющий диапазон<br/>который содержит область столбца в отчете сводной таблицы. Только для чтения.|
| [row_range](/cells/ru/python-net/aspose.cells.pivot/pivottable/row_range) | Возвращает объект CellArea, представляющий диапазон<br/> который содержит область строк в отчете сводной таблицы. Только для чтения.|
| [data_body_range](/cells/ru/python-net/aspose.cells.pivot/pivottable/data_body_range) | Возвращает объект CellArea, представляющий диапазон, содержащий область данных.<br/> в списке между строкой заголовка и строкой вставки. Только для чтения.|
| [table_range1](/cells/ru/python-net/aspose.cells.pivot/pivottable/table_range1) | Возвращает объект CellArea, представляющий диапазон, содержащий весь отчет сводной таблицы.<br/> но не включает поля страницы. Только для чтения.|
| [table_range2](/cells/ru/python-net/aspose.cells.pivot/pivottable/table_range2) | Возвращает объект CellArea, представляющий диапазон, содержащий весь отчет сводной таблицы.<br/> включает поля страницы. Только для чтения.|
| [column_grand](/cells/ru/python-net/aspose.cells.pivot/pivottable/column_grand) | Указывает, отображаются ли в отчете сводной таблицы общие итоги для столбцов.|
| [is_grid_drop_zones](/cells/ru/python-net/aspose.cells.pivot/pivottable/is_grid_drop_zones) | Указывает, отображает ли отчет сводной таблицы классический макет сводной таблицы.<br/> (позволяет перетаскивать поля в сетке)|
| [row_grand](/cells/ru/python-net/aspose.cells.pivot/pivottable/row_grand) | Указывает, отображаются ли в отчете сводной таблицы общие итоги для строк.|
| [display_null_string](/cells/ru/python-net/aspose.cells.pivot/pivottable/display_null_string) | Указывает, отображает ли отчет сводной таблицы настраиваемую строку.<br/> в ячейках, содержащих нулевые значения.|
| [null_string](/cells/ru/python-net/aspose.cells.pivot/pivottable/null_string) | Получает строку, отображаемую в ячейках, содержащих нулевые значения.<br/> когда свойство DisplayNullString имеет значение true. Значение по умолчанию — пустая строка.|
| [display_error_string](/cells/ru/python-net/aspose.cells.pivot/pivottable/display_error_string) | Указывает, отображает ли отчет сводной таблицы пользовательскую строку в ячейках, содержащих ошибки.|
| [data_field_header_name](/cells/ru/python-net/aspose.cells.pivot/pivottable/data_field_header_name) | Получает и задает имя заголовка поля области значений в сводной таблице.|
| [error_string](/cells/ru/python-net/aspose.cells.pivot/pivottable/error_string) | Получает строку, отображаемую в ячейках, содержащих ошибки<br/>когда свойство DisplayErrorString имеет значение true. Значением по умолчанию является пустая строка.|
| [is_auto_format](/cells/ru/python-net/aspose.cells.pivot/pivottable/is_auto_format) | Указывает, форматируется ли отчет сводной таблицы автоматически.<br/>Флажок «Автоформат таблицы», который находится в опции сводной таблицы для Excel 2003<br/> Флажок «автоподбор ширины столбца при обновлении», который находится в параметрах сводной таблицы: формат макета для Excel 2007|
| [auto_format_type](/cells/ru/python-net/aspose.cells.pivot/pivottable/auto_format_type) | Получает тип автоматического форматирования сводной таблицы.|
| [has_blank_rows](/cells/ru/python-net/aspose.cells.pivot/pivottable/has_blank_rows) | Указывает, добавлять ли пустые строки.<br/> Это свойство применяется только к типам автоматического форматирования сводных таблиц, которым необходимо добавлять пустые строки.|
| [merge_labels](/cells/ru/python-net/aspose.cells.pivot/pivottable/merge_labels) | Указывает, является ли указанный элемент внешней строки отчета сводной таблицы, элемент столбца, промежуточный итог,<br/> а метки общего итога используют объединенные ячейки.|
| [preserve_formatting](/cells/ru/python-net/aspose.cells.pivot/pivottable/preserve_formatting) | Указывает, сохраняется ли форматирование при обновлении или пересчете сводной таблицы.|
| [show_drill](/cells/ru/python-net/aspose.cells.pivot/pivottable/show_drill) | Получает, отображаются ли кнопки развертывания/свертывания.|
| [enable_drilldown](/cells/ru/python-net/aspose.cells.pivot/pivottable/enable_drilldown) | Получает, включена ли детализация.|
| [enable_field_dialog](/cells/ru/python-net/aspose.cells.pivot/pivottable/enable_field_dialog) | Указывает, доступно ли диалоговое окно поля сводной таблицы.<br/> когда пользователь дважды щелкает поле сводной таблицы.|
| [enable_field_list](/cells/ru/python-net/aspose.cells.pivot/pivottable/enable_field_list) | Получает, включает ли список полей для сводной таблицы.|
| [enable_wizard](/cells/ru/python-net/aspose.cells.pivot/pivottable/enable_wizard) | Указывает, доступен ли мастер сводных таблиц.|
| [subtotal_hidden_page_items](/cells/ru/python-net/aspose.cells.pivot/pivottable/subtotal_hidden_page_items) | Указывает, будут ли элементы поля скрытой страницы в отчете сводной таблицы<br/>включаются в промежуточные итоги строк и столбцов, итоги блоков и общие итоги.<br/> Значение по умолчанию неверно.|
| [grand_total_name](/cells/ru/python-net/aspose.cells.pivot/pivottable/grand_total_name) | Возвращает метку текстовой строки, отображаемую в заголовке столбца общей суммы или строки.<br/> Значением по умолчанию является строка «Общий итог».|
| [manual_update](/cells/ru/python-net/aspose.cells.pivot/pivottable/manual_update) | Указывает, пересчитывается ли отчет сводной таблицы только по запросу пользователя.|
| [is_multiple_field_filters](/cells/ru/python-net/aspose.cells.pivot/pivottable/is_multiple_field_filters) | Задает логическое значение, указывающее, могут ли поля сводной таблицы иметь несколько фильтров.|
| [missing_items_limit](/cells/ru/python-net/aspose.cells.pivot/pivottable/missing_items_limit) | Задает логическое значение, указывающее, могут ли поля сводной таблицы иметь несколько фильтров.|
| [enable_data_value_editing](/cells/ru/python-net/aspose.cells.pivot/pivottable/enable_data_value_editing) |Задает логическое значение, указывающее, разрешено ли пользователю редактировать ячейки в области данных сводной таблицы.<br/> Включить редактирование ячеек в области значений|
| [show_data_tips](/cells/ru/python-net/aspose.cells.pivot/pivottable/show_data_tips) | Указывает логическое значение, указывающее, должны ли отображаться всплывающие подсказки для ячеек данных сводной таблицы.|
| [show_member_property_tips](/cells/ru/python-net/aspose.cells.pivot/pivottable/show_member_property_tips) | Задает логическое значение, указывающее, следует ли исключить сведения о свойствах элементов из всплывающих подсказок сводной таблицы.|
| [show_values_row](/cells/ru/python-net/aspose.cells.pivot/pivottable/show_values_row) | Задает логическое значение, указывающее, следует ли отображать строку значений.<br/> показать строку значений|
| [show_empty_col](/cells/ru/python-net/aspose.cells.pivot/pivottable/show_empty_col) | Указывает логическое значение, указывающее, следует ли включать в таблицу пустые столбцы.|
| [show_empty_row](/cells/ru/python-net/aspose.cells.pivot/pivottable/show_empty_row) | Задает логическое значение, указывающее, следует ли включать в таблицу пустые строки.|
| [field_list_sort_ascending](/cells/ru/python-net/aspose.cells.pivot/pivottable/field_list_sort_ascending) | Указывает логическое значение, указывающее, сортируются ли поля в сводной таблице в порядке, отличном от порядка по умолчанию в списке полей.|
| [print_drill](/cells/ru/python-net/aspose.cells.pivot/pivottable/print_drill) | Задает логическое значение, указывающее, следует ли печатать индикаторы детализации.<br/> печатать кнопки развертывания/свертывания при отображении в сводной таблице.|
| [alt_text_title](/cells/ru/python-net/aspose.cells.pivot/pivottable/alt_text_title) | Получает заголовок альтертекста|
| [alt_text_description](/cells/ru/python-net/aspose.cells.pivot/pivottable/alt_text_description) | Получает описание альтернативного текста|
| [name](/cells/ru/python-net/aspose.cells.pivot/pivottable/name) | Получает имя сводной таблицы|
| [column_header_caption](/cells/ru/python-net/aspose.cells.pivot/pivottable/column_header_caption) | Получает заголовок заголовка столбца сводной таблицы.|
| [indent](/cells/ru/python-net/aspose.cells.pivot/pivottable/indent) | Указывает приращение отступа для компактной оси и может использоваться для установки макета отчета в компактную форму.|
| [row_header_caption](/cells/ru/python-net/aspose.cells.pivot/pivottable/row_header_caption) | Получает заголовок строки сводной таблицы.|
| [show_row_header_caption](/cells/ru/python-net/aspose.cells.pivot/pivottable/show_row_header_caption) | Указывает, отображается ли заголовок строки в отчете сводной таблицы.<br/> Указывает, будут ли отображаться заголовки полей и раскрывающиеся списки фильтров.|
| [custom_list_sort](/cells/ru/python-net/aspose.cells.pivot/pivottable/custom_list_sort) | Указывает, следует ли учитывать встроенный настраиваемый список при сортировке данных.|
| [pivot_format_conditions](/cells/ru/python-net/aspose.cells.pivot/pivottable/pivot_format_conditions) | Получает условия формата сводной таблицы.|
| [page_field_order](/cells/ru/python-net/aspose.cells.pivot/pivottable/page_field_order) |Получает порядок, в котором поля страницы добавляются в макет отчета сводной таблицы.|
| [page_field_wrap_count](/cells/ru/python-net/aspose.cells.pivot/pivottable/page_field_wrap_count) | Получает количество полей страницы в каждом столбце или строке отчета сводной таблицы.|
| [tag](/cells/ru/python-net/aspose.cells.pivot/pivottable/tag) | Получает строку, сохраненную в отчете сводной таблицы.|
| [save_data](/cells/ru/python-net/aspose.cells.pivot/pivottable/save_data) | Указывает, сохраняются ли данные для отчета сводной таблицы вместе с книгой.|
| [refresh_data_on_opening_file](/cells/ru/python-net/aspose.cells.pivot/pivottable/refresh_data_on_opening_file) | Указывает, следует ли обновлять данные при открытии файла.|
| [refresh_data_flag](/cells/ru/python-net/aspose.cells.pivot/pivottable/refresh_data_flag) | Указывает, следует ли обновлять данные или нет.|
| [external_connection_data_source](/cells/ru/python-net/aspose.cells.pivot/pivottable/external_connection_data_source) | Получает источник данных внешнего подключения.|
| [data_source](/cells/ru/python-net/aspose.cells.pivot/pivottable/data_source) | Получает и задает источник данных сводной таблицы.|
| [item_print_titles](/cells/ru/python-net/aspose.cells.pivot/pivottable/item_print_titles) | Бит, указывающий, будут ли заголовки сводных элементов на оси строки<br/> повторяются на каждой печатной странице для сводных полей в табличной форме.|
| [print_titles](/cells/ru/python-net/aspose.cells.pivot/pivottable/print_titles) | Указывает, установлены ли печатные заголовки рабочего листа на основе<br/> в отчете сводной таблицы. Значение по умолчанию неверно.|
| [display_immediate_items](/cells/ru/python-net/aspose.cells.pivot/pivottable/display_immediate_items) | Указывает, видны ли элементы в области строк и столбцов.<br/> когда область данных сводной таблицы пуста. Значение по умолчанию верно.|
| [is_selected](/cells/ru/python-net/aspose.cells.pivot/pivottable/is_selected) | Указывает, выбрана ли сводная таблица.|
| [show_pivot_style_row_header](/cells/ru/python-net/aspose.cells.pivot/pivottable/show_pivot_style_row_header) |Указывает, следует ли применять стиль к заголовку строки в сводной таблице.|
| [show_pivot_style_column_header](/cells/ru/python-net/aspose.cells.pivot/pivottable/show_pivot_style_column_header) | Указывает, следует ли применять стиль к заголовку столбца в сводной таблице.|
| [show_pivot_style_row_stripes](/cells/ru/python-net/aspose.cells.pivot/pivottable/show_pivot_style_row_stripes) | Указывает, применяется ли форматирование чередования строк.|
| [show_pivot_style_column_stripes](/cells/ru/python-net/aspose.cells.pivot/pivottable/show_pivot_style_column_stripes) | Указывает, применяется ли форматирование чередования столбцов.|
| [show_pivot_style_last_column](/cells/ru/python-net/aspose.cells.pivot/pivottable/show_pivot_style_last_column) | Указывает, применяется ли форматирование чередования столбцов.|


###  Методы
| Метод| Описание|
| :- | :- |
| [remove_field(field_type, field_name)](/cells/ru/python-net/aspose.cells.pivot/pivottable/remove_field/#PivotFieldType-str) | Удаляет поле из определенной области поля|
| [remove_field(field_type, base_field_index)](/cells/ru/python-net/aspose.cells.pivot/pivottable/remove_field/#PivotFieldType-int) | Удаляет поле из определенной области поля|
| [remove_field(field_type, pivot_field)](/cells/ru/python-net/aspose.cells.pivot/pivottable/remove_field/#PivotFieldType-PivotField) | Удалить поле из определенной области поля|
| [add_field_to_area(field_type, field_name)](/cells/ru/python-net/aspose.cells.pivot/pivottable/add_field_to_area/#PivotFieldType-str) | Добавляет поле в определенную область.|
| [add_field_to_area(field_type, base_field_index)](/cells/ru/python-net/aspose.cells.pivot/pivottable/add_field_to_area/#PivotFieldType-int) | Добавляет поле в определенную область.|
| [add_field_to_area(field_type, pivot_field)](/cells/ru/python-net/aspose.cells.pivot/pivottable/add_field_to_area/#PivotFieldType-PivotField) | Добавляет поле в определенную область.|
| [add_calculated_field(name, formula, drag_to_data_area)](/cells/ru/python-net/aspose.cells.pivot/pivottable/add_calculated_field/#str-str-bool) | Добавляет вычисляемое поле в сводное поле.|
| [add_calculated_field(name, formula)](/cells/ru/python-net/aspose.cells.pivot/pivottable/add_calculated_field/#str-str) |Добавляет вычисляемое поле в сводное поле и перетаскивает его в область данных.|
| [move(row, column)](/cells/ru/python-net/aspose.cells.pivot/pivottable/move/#int-int) | Перемещает сводную таблицу в другое место на листе.|
| [move(dest_cell_name)](/cells/ru/python-net/aspose.cells.pivot/pivottable/move/#str) | Перемещает сводную таблицу в другое место на листе.|
| [set_auto_group_field(base_field_index)](/cells/ru/python-net/aspose.cells.pivot/pivottable/set_auto_group_field/#int) | Задает группу автоматических полей по сводной таблице.|
| [set_auto_group_field(pivot_field)](/cells/ru/python-net/aspose.cells.pivot/pivottable/set_auto_group_field/#PivotField) | Задает группу автоматических полей по сводной таблице.|
| [set_manual_group_field(base_field_index, start_val, end_val, group_by_list, interval_num)](/cells/ru/python-net/aspose.cells.pivot/pivottable/set_manual_group_field/#int-float-float-list-float) | Задает группу полей вручную для сводной таблицы.|
| [set_manual_group_field(pivot_field, start_val, end_val, group_by_list, interval_num)](/cells/ru/python-net/aspose.cells.pivot/pivottable/set_manual_group_field/#PivotField-float-float-list-float) | Задает группу полей вручную для сводной таблицы.|
| [set_manual_group_field(base_field_index, start_val, end_val, group_by_list, interval_num)](/cells/ru/python-net/aspose.cells.pivot/pivottable/set_manual_group_field/#int-DateTime-DateTime-list-int) | Задает группу полей вручную для сводной таблицы.|
| [set_manual_group_field(pivot_field, start_val, end_val, group_by_list, interval_num)](/cells/ru/python-net/aspose.cells.pivot/pivottable/set_manual_group_field/#PivotField-DateTime-DateTime-list-int) | Задает группу полей вручную для сводной таблицы.|
| [set_ungroup(base_field_index)](/cells/ru/python-net/aspose.cells.pivot/pivottable/set_ungroup/#int) | Устанавливает разгруппировку по сводной таблице|
| [set_ungroup(pivot_field)](/cells/ru/python-net/aspose.cells.pivot/pivottable/set_ungroup/#PivotField) | Устанавливает разгруппировку по сводной таблице|
| [copy_style(pivot_table)](/cells/ru/python-net/aspose.cells.pivot/pivottable/copy_style/#PivotTable) | Копирует именованный стиль из другой сводной таблицы.|
| [show_report_filter_page(page_field)](/cells/ru/python-net/aspose.cells.pivot/pivottable/show_report_filter_page/#PivotField) | Показать все страницы фильтра отчета в соответствии с PivotField, PivotField должен находиться в PageFields.|
| [show_report_filter_page_by_name(field_name)](/cells/ru/python-net/aspose.cells.pivot/pivottable/show_report_filter_page_by_name/#str) | Показать все страницы фильтра отчетов в соответствии с именем PivotField, PivotField должен находиться в PageFields.|
| [show_report_filter_page_by_index(pos_index)](/cells/ru/python-net/aspose.cells.pivot/pivottable/show_report_filter_page_by_index/#int) | Показать все страницы фильтра отчета в соответствии с индексом позиции в PageFields|
| [fields(field_type)](/cells/ru/python-net/aspose.cells.pivot/pivottable/fields/#PivotFieldType) | Получает определенные поля по типу поля.|
| [change_data_source(source)](/cells/ru/python-net/aspose.cells.pivot/pivottable/change_data_source/#list) |Установите исходные данные сводной таблицы.<br/> Лист1!$A$1:$C$3|
| [get_source()](/cells/ru/python-net/aspose.cells.pivot/pivottable/get_source/#) | Получить исходные данные сводной таблицы.|
| [refresh_data()](/cells/ru/python-net/aspose.cells.pivot/pivottable/refresh_data/#) | Обновляет данные сводной таблицы и настройки из ее источника данных.|
| [calculate_data()](/cells/ru/python-net/aspose.cells.pivot/pivottable/calculate_data/#) | Вычисляет данные сводной таблицы в ячейки.|
| [clear_data()](/cells/ru/python-net/aspose.cells.pivot/pivottable/clear_data/#) | Очистить данные и форматирование сводной таблицы|
| [calculate_range()](/cells/ru/python-net/aspose.cells.pivot/pivottable/calculate_range/#) | Вычисляет диапазон сводной таблицы.|
| [format_all(style)](/cells/ru/python-net/aspose.cells.pivot/pivottable/format_all/#Style) | Отформатировать всю ячейку в сводной области|
| [format_row(row, style)](/cells/ru/python-net/aspose.cells.pivot/pivottable/format_row/#int-Style) | Форматирование данных строки в области сводной таблицы|
| [format(row, column, style)](/cells/ru/python-net/aspose.cells.pivot/pivottable/format/#int-int-Style) | Отформатируйте ячейку в сводной области|
| [get_horizontal_breaks()](/cells/ru/python-net/aspose.cells.pivot/pivottable/get_horizontal_breaks/#) | получить список индексов строк сводной таблицы горизонтальных разрывов страниц|
| [show_in_compact_form()](/cells/ru/python-net/aspose.cells.pivot/pivottable/show_in_compact_form/#) |Макеты сводной таблицы в компактной форме.|
| [show_in_outline_form()](/cells/ru/python-net/aspose.cells.pivot/pivottable/show_in_outline_form/#) | Макеты сводной таблицы в виде схемы.|
| [show_in_tabular_form()](/cells/ru/python-net/aspose.cells.pivot/pivottable/show_in_tabular_form/#) | Макеты сводной таблицы в табличной форме.|
| [get_cell_by_display_name(display_name)](/cells/ru/python-net/aspose.cells.pivot/pivottable/get_cell_by_display_name/#str) | Получает объект Cell по DisplayName поля PivotField.|
| [get_children()](/cells/ru/python-net/aspose.cells.pivot/pivottable/get_children/#) |Получает дочерние сводные таблицы, которые используют данные этой сводной таблицы в качестве источника данных.|



###  Пример

```python
from aspose.cells import FormatConditionType, OperatorType, Workbook
from aspose.cells.pivot import PivotFieldType, PivotFilterType, PivotTableStyleType
from aspose.pydrawing import Color

book = Workbook()
sheet = book.worksheets[0]
cells = sheet.cells
cells.get(0, 0).value = "fruit"
cells.get(1, 0).value = "grape"
cells.get(2, 0).value = "blueberry"
cells.get(3, 0).value = "kiwi"
cells.get(4, 0).value = "cherry"
cells.get(5, 0).value = "grape"
cells.get(6, 0).value = "blueberry"
cells.get(7, 0).value = "kiwi"
cells.get(8, 0).value = "cherry"
cells.get(0, 1).value = "year"
cells.get(1, 1).value = 2020
cells.get(2, 1).value = 2020
cells.get(3, 1).value = 2020
cells.get(4, 1).value = 2020
cells.get(5, 1).value = 2021
cells.get(6, 1).value = 2021
cells.get(7, 1).value = 2021
cells.get(8, 1).value = 2021
cells.get(0, 2).value = "amount"
cells.get(1, 2).value = 50
cells.get(2, 2).value = 60
cells.get(3, 2).value = 70
cells.get(4, 2).value = 80
cells.get(5, 2).value = 90
cells.get(6, 2).value = 100
cells.get(7, 2).value = 110
cells.get(8, 2).value = 120
pivots = sheet.pivot_tables
pivotIndex = pivots.add("=Sheet1!A1:C9", "A12", "TestPivotTable")
pivot = pivots[pivotIndex]
pivot.add_field_to_area(PivotFieldType.ROW, "fruit")
pivot.add_field_to_area(PivotFieldType.COLUMN, "year")
pivot.add_field_to_area(PivotFieldType.DATA, "amount")
pivot.pivot_table_style_type = PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM10
# Change PivotField's attributes
rowField = pivot.row_fields[0]
rowField.display_name = "custom display name"
# Add PivotFilter
index = pivot.pivot_filters.add(0, PivotFilterType.COUNT)
filter = pivot.pivot_filters[index]
filter.auto_filter.filter_top10(0, False, False, 2)
# Add PivotFormatCondition
formatIndex = pivot.pivot_format_conditions.add()
pfc = pivot.pivot_format_conditions[formatIndex]
fcc = pfc.format_conditions
fcc.add_area(pivot.data_body_range)
idx = fcc.add_condition(FormatConditionType.CELL_VALUE)
fc = fcc[idx]
fc.formula1 = "100"
fc.operator = OperatorType.GREATER_OR_EQUAL
fc.style.background_color = Color.red
pivot.refresh_data()
pivot.calculate_data()
# do your business
book.save("out.xlsx")

```

###  Смотрите также
* модуль [aspose.cells.pivot](..)
