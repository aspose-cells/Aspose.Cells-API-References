---
title: Cells класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 180
url: /ru/python-net/aspose.cells/cells/
is_root: false
---
##  Cells класс
Инкапсулирует набор объектов, относящихся к ячейке, таких как [Cell](/cells/ru/python-net/aspose.cells/cell), [Row](/cells/ru/python-net/aspose.cells/row) и т. д.



Тип Cells предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [ods_cell_fields](/cells/ru/python-net/aspose.cells/cells/ods_cell_fields) | Получает список полей коэффициентов.|
| [count](/cells/ru/python-net/aspose.cells/cells/count) | Получает общее количество созданных объектов Cell.|
| [count_large](/cells/ru/python-net/aspose.cells/cells/count_large) | Получает общее количество созданных объектов Cell.|
| [rows](/cells/ru/python-net/aspose.cells/cells/rows) | Получает коллекцию из [Row](/cells/ru/python-net/aspose.cells/row) объектов, представляющих отдельные строки на этом листе.|
| [merged_cells](/cells/ru/python-net/aspose.cells/cells/merged_cells) | Получает коллекцию объединенных ячеек.|
| [multi_thread_reading](/cells/ru/python-net/aspose.cells/cells/multi_thread_reading) | Получает или задает, должна ли модель данных ячеек поддерживать многопоточное чтение.<br/> Значение по умолчанию этого свойства — false.|
| [memory_setting](/cells/ru/python-net/aspose.cells/cells/memory_setting) | Получает или задает параметр использования памяти для этой ячейки.|
| [style](/cells/ru/python-net/aspose.cells/cells/style) | Получает и задает стиль по умолчанию.|
| [standard_width_inch](/cells/ru/python-net/aspose.cells/cells/standard_width_inch) |Получает или задает ширину столбца по умолчанию на листе в дюймах.|
| [standard_width_pixels](/cells/ru/python-net/aspose.cells/cells/standard_width_pixels) | Получает или задает ширину столбца по умолчанию на листе в пикселях.|
| [standard_width](/cells/ru/python-net/aspose.cells/cells/standard_width) | Получает или задает ширину столбца по умолчанию на листе в символьных единицах.|
| [standard_height](/cells/ru/python-net/aspose.cells/cells/standard_height) | Получает или задает высоту строки по умолчанию на этом листе в пунктах.|
| [standard_height_pixels](/cells/ru/python-net/aspose.cells/cells/standard_height_pixels) | Получает или задает высоту строки по умолчанию на этом листе в пикселях.|
| [standard_height_inch](/cells/ru/python-net/aspose.cells/cells/standard_height_inch) | Получает или задает высоту строки по умолчанию на этом листе в дюймах.|
| [preserve_string](/cells/ru/python-net/aspose.cells/cells/preserve_string) | Получает или задает значение, указывающее, сохраняются ли все значения рабочего листа в виде строк.<br/> Значение по умолчанию — ложь.|
| [min_row](/cells/ru/python-net/aspose.cells/cells/min_row) | Минимальный индекс строки ячейки, содержащей данные или стиль.|
| [max_row](/cells/ru/python-net/aspose.cells/cells/max_row) | Максимальный индекс строки ячейки, содержащей данные или стиль.|
| [min_column](/cells/ru/python-net/aspose.cells/cells/min_column) | Минимальный индекс столбца тех ячеек, которые были созданы в коллекции (не включает столбец<br/> где стиль определен для всего столбца, но в нем не создана ни одна ячейка).|
| [max_column](/cells/ru/python-net/aspose.cells/cells/max_column) | Минимальный индекс столбца тех ячеек, которые были созданы в коллекции (не включает столбец<br/> где стиль определен для всего столбца, но в нем не создана ни одна ячейка).|
| [min_data_row](/cells/ru/python-net/aspose.cells/cells/min_data_row) | Минимальный индекс строки ячейки, содержащей данные.|
| [max_data_row](/cells/ru/python-net/aspose.cells/cells/max_data_row) |Максимальный индекс строки ячейки, содержащей данные.|
| [min_data_column](/cells/ru/python-net/aspose.cells/cells/min_data_column) | Минимальный индекс столбца ячейки, содержащей данные.|
| [max_data_column](/cells/ru/python-net/aspose.cells/cells/max_data_column) | Максимальный индекс столбца ячейки, содержащей данные.|
| [is_default_row_height_matched](/cells/ru/python-net/aspose.cells/cells/is_default_row_height_matched) | Указывает, что высота строки и высота шрифта по умолчанию совпадают.|
| [is_default_row_hidden](/cells/ru/python-net/aspose.cells/cells/is_default_row_hidden) | Указывает, скрыта ли строка по умолчанию.|
| [columns](/cells/ru/python-net/aspose.cells/cells/columns) | Получает коллекцию из [Column](/cells/ru/python-net/aspose.cells/column) объектов, представляющих отдельные столбцы на этом листе.|
| [ranges](/cells/ru/python-net/aspose.cells/cells/ranges) | Получает коллекцию из [Range](/cells/ru/python-net/aspose.cells/range) объектов, созданных во время выполнения.|
| [last_cell](/cells/ru/python-net/aspose.cells/cells/last_cell) | Получает последнюю ячейку на этом листе.|
| [max_display_range](/cells/ru/python-net/aspose.cells/cells/max_display_range) | Получает максимальный диапазон, включающий данные, объединенные ячейки и фигуры.|
| [first_cell](/cells/ru/python-net/aspose.cells/cells/first_cell) | Получает первую ячейку на этом листе.|



Получает элемент [Cell](/cells/ru/python-net/aspose.cells/cell) на листе
###  Индексатор
| Имя| Описание|
| :- | :- |
| [index] | Отсчитываемый от нуля индекс элемента.|


###  Методы
| Метод| Описание|
| :- | :- |
| [create_range(upper_left_cell, lower_right_cell)](/cells/ru/python-net/aspose.cells/cells/create_range/#str-str) | Создает объект [Range](/cells/ru/python-net/aspose.cells/range) из диапазона ячеек.|
| [create_range(first_row, first_column, total_rows, total_columns)](/cells/ru/python-net/aspose.cells/cells/create_range/#int-int-int-int) | Создает объект [Range](/cells/ru/python-net/aspose.cells/range) из диапазона ячеек.|
| [create_range(address)](/cells/ru/python-net/aspose.cells/cells/create_range/#str) | Создает объект [Range](/cells/ru/python-net/aspose.cells/range) из адреса диапазона.|
| [create_range(first_index, number, is_vertical)](/cells/ru/python-net/aspose.cells/cells/create_range/#int-int-bool) | Создает объект [Range](/cells/ru/python-net/aspose.cells/range) из строк ячеек или столбцов ячеек.|
| [get(row, column)](/cells/ru/python-net/aspose.cells/cells/get/#int-int) |Добавить API for Python через .Net.так как это [int row, int column] не поддерживается|
| [get(cell_name)](/cells/ru/python-net/aspose.cells/cells/get/#str) | Добавить API for Python через .Net.так как это [string cellName] не поддерживается|
| [import_object_array(obj_array, first_row, first_column, is_vertical)](/cells/ru/python-net/aspose.cells/cells/import_object_array/#list-int-int-bool) | Импортирует массив данных на рабочий лист.|
| [import_object_array(obj_array, first_row, first_column, is_vertical, skip)](/cells/ru/python-net/aspose.cells/cells/import_object_array/#list-int-int-bool-int) | Импортирует массив данных на рабочий лист.|
| [import_array(string_array, first_row, first_column, is_vertical)](/cells/ru/python-net/aspose.cells/cells/import_array/#list-int-int-bool) | Импортирует массив строк на рабочий лист.|
| [import_array(int_array, first_row, first_column, is_vertical)](/cells/ru/python-net/aspose.cells/cells/import_array/#list-int-int-bool) | Импортирует массив целых чисел на лист.|
| [import_array(double_array, first_row, first_column, is_vertical)](/cells/ru/python-net/aspose.cells/cells/import_array/#list-int-int-bool) | Импортирует массив двойников на лист.|
| [import_csv(file_name, splitter, convert_numeric_data, first_row, first_column)](/cells/ru/python-net/aspose.cells/cells/import_csv/#str-str-bool-int-int) | Импортируйте файл CSV в ячейки.|
| [import_csv(stream, splitter, convert_numeric_data, first_row, first_column)](/cells/ru/python-net/aspose.cells/cells/import_csv/#io.RawIOBase-str-bool-int-int) | Импортируйте файл CSV в ячейки.|
| [import_csv(file_name, options, first_row, first_column)](/cells/ru/python-net/aspose.cells/cells/import_csv/#str-TxtLoadOptions-int-int) | Импортируйте файл CSV в ячейки.|
| [import_csv(stream, options, first_row, first_column)](/cells/ru/python-net/aspose.cells/cells/import_csv/#io.RawIOBase-TxtLoadOptions-int-int) | Импортируйте файл CSV в ячейки.|
| [merge(first_row, first_column, total_rows, total_columns)](/cells/ru/python-net/aspose.cells/cells/merge/#int-int-int-int) | Объединяет указанный диапазон ячеек в одну ячейку.|
| [merge(first_row, first_column, total_rows, total_columns, merge_conflict)](/cells/ru/python-net/aspose.cells/cells/merge/#int-int-int-int-bool) | Объединяет указанный диапазон ячеек в одну ячейку.|
| [merge(first_row, first_column, total_rows, total_columns, check_conflict, merge_conflict)](/cells/ru/python-net/aspose.cells/cells/merge/#int-int-int-int-bool-bool) | Объединяет указанный диапазон ячеек в одну ячейку.|
| [copy_columns(source_cells0, source_column_index, destination_column_index, column_number, paste_options)](/cells/ru/python-net/aspose.cells/cells/copy_columns/#Cells-int-int-int-PasteOptions) | Копирует данные и форматы всего столбца.|
| [copy_columns(source_cells0, source_column_index, destination_column_index, column_number)](/cells/ru/python-net/aspose.cells/cells/copy_columns/#Cells-int-int-int) | Копирует данные и форматы всего столбца.|
| [copy_columns(source_cells, source_column_index, source_total_columns, destination_column_index, destination_total_columns)](/cells/ru/python-net/aspose.cells/cells/copy_columns/#Cells-int-int-int-int) | Копирует данные и форматы целых столбцов.|
| [copy_rows(source_cells, source_row_index, destination_row_index, row_number)](/cells/ru/python-net/aspose.cells/cells/copy_rows/#Cells-int-int-int) | Копирует данные и форматы некоторых целых строк.|
| [copy_rows(source_cells0, source_row_index, destination_row_index, row_number, copy_options)](/cells/ru/python-net/aspose.cells/cells/copy_rows/#Cells-int-int-int-CopyOptions) | Копирует данные и форматы некоторых целых строк.|
| [copy_rows(source_cells0, source_row_index, destination_row_index, row_number, copy_options, paste_options)](/cells/ru/python-net/aspose.cells/cells/copy_rows/#Cells-int-int-int-CopyOptions-PasteOptions) | Копирует данные и форматы некоторых целых строк.|
| [group_columns(first_index, last_index)](/cells/ru/python-net/aspose.cells/cells/group_columns/#int-int) | Групповые столбцы.|
| [group_columns(first_index, last_index, is_hidden)](/cells/ru/python-net/aspose.cells/cells/group_columns/#int-int-bool) | Групповые столбцы.|
| [ungroup_rows(first_index, last_index, is_all)](/cells/ru/python-net/aspose.cells/cells/ungroup_rows/#int-int-bool) | Разгруппировать строки.|
| [ungroup_rows(first_index, last_index)](/cells/ru/python-net/aspose.cells/cells/ungroup_rows/#int-int) | Разгруппировать строки.|
| [group_rows(first_index, last_index, is_hidden)](/cells/ru/python-net/aspose.cells/cells/group_rows/#int-int-bool) | Группирует строки.|
| [group_rows(first_index, last_index)](/cells/ru/python-net/aspose.cells/cells/group_rows/#int-int) | Группирует строки.|
| [delete_column(column_index, update_reference)](/cells/ru/python-net/aspose.cells/cells/delete_column/#int-bool) | Удаляет столбец.|
| [delete_column(column_index)](/cells/ru/python-net/aspose.cells/cells/delete_column/#int) | Удаляет столбец.|
| [delete_rows(row_index, total_rows)](/cells/ru/python-net/aspose.cells/cells/delete_rows/#int-int) | Удаляет несколько строк.|
| [delete_rows(row_index, total_rows, update_reference)](/cells/ru/python-net/aspose.cells/cells/delete_rows/#int-int-bool) | Удаляет несколько строк на листе.|
| [delete_blank_columns()](/cells/ru/python-net/aspose.cells/cells/delete_blank_columns/#) | Удалите все пустые столбцы, которые не содержат данных.|
| [delete_blank_columns(options)](/cells/ru/python-net/aspose.cells/cells/delete_blank_columns/#DeleteOptions) | Удалите все пустые столбцы, которые не содержат данных.|
| [delete_blank_rows()](/cells/ru/python-net/aspose.cells/cells/delete_blank_rows/#) | Удалите все пустые строки, которые не содержат данных.|
| [delete_blank_rows(options)](/cells/ru/python-net/aspose.cells/cells/delete_blank_rows/#DeleteOptions) | Удалите все пустые строки, которые не содержат данных.|
| [insert_columns(column_index, total_columns)](/cells/ru/python-net/aspose.cells/cells/insert_columns/#int-int) | Вставляет несколько столбцов в рабочий лист.|
| [insert_columns(column_index, total_columns, update_reference)](/cells/ru/python-net/aspose.cells/cells/insert_columns/#int-int-bool) | Вставляет несколько столбцов в рабочий лист.|
| [insert_column(column_index, update_reference)](/cells/ru/python-net/aspose.cells/cells/insert_column/#int-bool) |Вставляет новый столбец в рабочий лист.|
| [insert_column(column_index)](/cells/ru/python-net/aspose.cells/cells/insert_column/#int) |Вставляет новый столбец в рабочий лист.|
| [insert_rows(row_index, total_rows, update_reference)](/cells/ru/python-net/aspose.cells/cells/insert_rows/#int-int-bool) | Вставляет несколько строк в рабочий лист.|
| [insert_rows(row_index, total_rows, options)](/cells/ru/python-net/aspose.cells/cells/insert_rows/#int-int-InsertOptions) | Вставляет несколько строк в рабочий лист.|
| [insert_rows(row_index, total_rows)](/cells/ru/python-net/aspose.cells/cells/insert_rows/#int-int) | Вставляет несколько строк в рабочий лист.|
| [clear_range(range)](/cells/ru/python-net/aspose.cells/cells/clear_range/#CellArea) | Очищает содержимое и форматирование диапазона.|
| [clear_range(start_row, start_column, end_row, end_column)](/cells/ru/python-net/aspose.cells/cells/clear_range/#int-int-int-int) | Очищает содержимое и форматирование диапазона.|
| [clear_contents(range)](/cells/ru/python-net/aspose.cells/cells/clear_contents/#CellArea) | Очищает содержимое диапазона.|
| [clear_contents(start_row, start_column, end_row, end_column)](/cells/ru/python-net/aspose.cells/cells/clear_contents/#int-int-int-int) | Очищает содержимое диапазона.|
| [clear_formats(range)](/cells/ru/python-net/aspose.cells/cells/clear_formats/#CellArea) | Очищает форматирование диапазона.|
| [clear_formats(start_row, start_column, end_row, end_column)](/cells/ru/python-net/aspose.cells/cells/clear_formats/#int-int-int-int) | Очищает форматирование диапазона.|
| [find(what, previous_cell)](/cells/ru/python-net/aspose.cells/cells/find/#any-Cell) | Находит ячейку, содержащую входной объект.|
| [find(what, previous_cell, find_options)](/cells/ru/python-net/aspose.cells/cells/find/#any-Cell-FindOptions) | Находит ячейку, содержащую входной объект.|
| [end_cell_in_row(row_index)](/cells/ru/python-net/aspose.cells/cells/end_cell_in_row/#int) | Получает последнюю ячейку в этой строке.|
| [end_cell_in_row(start_row, end_row, start_column, end_column)](/cells/ru/python-net/aspose.cells/cells/end_cell_in_row/#int-int-int-int) | Получает последнюю ячейку с максимальным индексом строки в этом диапазоне.|
| [end_cell_in_column(column_index)](/cells/ru/python-net/aspose.cells/cells/end_cell_in_column/#int) | Получает последнюю ячейку в этом столбце.|
| [end_cell_in_column(start_row, end_row, start_column, end_column)](/cells/ru/python-net/aspose.cells/cells/end_cell_in_column/#int-int-int-int) | Получает последнюю ячейку с максимальным индексом столбца в этом диапазоне.|
| [insert_range(area, shift_number, shift_type, update_reference)](/cells/ru/python-net/aspose.cells/cells/insert_range/#CellArea-int-ShiftType-bool) | Вставляет диапазон ячеек и сдвигает ячейки в соответствии с параметром сдвига.|
| [insert_range(area, shift_type)](/cells/ru/python-net/aspose.cells/cells/insert_range/#CellArea-ShiftType) | Вставляет диапазон ячеек и сдвигает ячейки в соответствии с параметром сдвига.|
| [insert_range(area, shift_number, shift_type)](/cells/ru/python-net/aspose.cells/cells/insert_range/#CellArea-int-ShiftType) | Вставляет диапазон ячеек и сдвигает ячейки в соответствии с параметром сдвига.|
| [import_custom_objects(list, property_names, is_property_name_shown, first_row, first_column, row_number, insert_rows, date_format_string, convert_string_to_number)](/cells/ru/python-net/aspose.cells/cells/import_custom_objects/#list-list-bool-int-int-int-bool-str-bool) | Импортирует пользовательские объекты.|
| [import_custom_objects(list, first_row, first_column, options)](/cells/ru/python-net/aspose.cells/cells/import_custom_objects/#list-int-int-ImportTableOptions) | Импортирует пользовательские объекты.|
| [subtotal(ca, group_by, function, total_list)](/cells/ru/python-net/aspose.cells/cells/subtotal/#CellArea-int-ConsolidationFunction-list) | Создает промежуточные итоги для диапазона.|
| [subtotal(ca, group_by, function, total_list, replace, page_breaks, summary_below_data)](/cells/ru/python-net/aspose.cells/cells/subtotal/#CellArea-int-ConsolidationFunction-list-bool-bool-bool) | Создает промежуточные итоги для диапазона.|
| [remove_duplicates()](/cells/ru/python-net/aspose.cells/cells/remove_duplicates/#) | Удаляет повторяющиеся строки в таблице.|
| [remove_duplicates(start_row, start_column, end_row, end_column)](/cells/ru/python-net/aspose.cells/cells/remove_duplicates/#int-int-int-int) | Удаляет повторяющиеся значения в диапазоне.|
| [remove_duplicates(start_row, start_column, end_row, end_column, has_headers, column_offsets)](/cells/ru/python-net/aspose.cells/cells/remove_duplicates/#int-int-int-int-bool-list) | Удаляет повторяющиеся данные диапазона.|
| [get_row_enumerator()](/cells/ru/python-net/aspose.cells/cells/get_row_enumerator/#) | Получает перечислитель строк.|
| [get_cell(row, column)](/cells/ru/python-net/aspose.cells/cells/get_cell/#int-int) | Получает элемент [Cell](/cells/ru/python-net/aspose.cells/cell) или значение NULL по указанному индексу строки ячейки и индексу столбца.|
| [get_row(row)](/cells/ru/python-net/aspose.cells/cells/get_row/#int) | Получает элемент [Row](/cells/ru/python-net/aspose.cells/row) по указанному индексу строки ячейки.|
| [check_cell(row, column)](/cells/ru/python-net/aspose.cells/cells/check_cell/#int-int) | Получает элемент [Cell](/cells/ru/python-net/aspose.cells/cell) или значение NULL по указанному индексу строки ячейки и индексу столбца.|
| [check_row(row)](/cells/ru/python-net/aspose.cells/cells/check_row/#int) |Получает элемент [Row](/cells/ru/python-net/aspose.cells/row) или указанный индекс строки ячейки.|
| [check_column(column_index)](/cells/ru/python-net/aspose.cells/cells/check_column/#int) | Получает элемент [Column](/cells/ru/python-net/aspose.cells/column) или null по указанному индексу столбца.|
| [is_row_hidden(row_index)](/cells/ru/python-net/aspose.cells/cells/is_row_hidden/#int) | Проверяет, скрыта ли строка по данному индексу.|
| [is_column_hidden(column_index)](/cells/ru/python-net/aspose.cells/cells/is_column_hidden/#int) | Проверяет, скрыт ли столбец с заданным индексом.|
| [add_range(range_object)](/cells/ru/python-net/aspose.cells/cells/add_range/#Range) | Добавляет ссылку на объект диапазона в ячейки|
| [clear()](/cells/ru/python-net/aspose.cells/cells/clear/#) | Очищает все объекты ячеек и строк.|
| [import_data(table, first_row, first_column, options)](/cells/ru/python-net/aspose.cells/cells/import_data/#ICellsDataTable-int-int-ImportTableOptions) | Импорт данных из пользовательской таблицы данных.|
| [import_array_list(array_list, first_row, first_column, is_vertical)](/cells/ru/python-net/aspose.cells/cells/import_array_list/#list-int-int-bool) | Импортирует массив данных на рабочий лист.|
| [import_formula_array(string_array, first_row, first_column, is_vertical)](/cells/ru/python-net/aspose.cells/cells/import_formula_array/#list-int-int-bool) | Импортирует массив формул на лист.|
| [text_to_columns(row, column, total_rows, options)](/cells/ru/python-net/aspose.cells/cells/text_to_columns/#int-int-int-TxtLoadOptions) | Разбивает текст в столбцах на столбцы.|
| [un_merge(first_row, first_column, total_rows, total_columns)](/cells/ru/python-net/aspose.cells/cells/un_merge/#int-int-int-int) | Разъединяет указанный диапазон объединенных ячеек.|
| [clear_merged_cells()](/cells/ru/python-net/aspose.cells/cells/clear_merged_cells/#) | Очищает все объединенные диапазоны.|
| [hide_row(row)](/cells/ru/python-net/aspose.cells/cells/hide_row/#int) | Скрывает ряд.|
| [unhide_row(row, height)](/cells/ru/python-net/aspose.cells/cells/unhide_row/#int-float) | Отобразить строку.|
| [hide_rows(row, total_rows)](/cells/ru/python-net/aspose.cells/cells/hide_rows/#int-int) | Скрывает несколько строк.|
| [unhide_rows(row, total_rows, height)](/cells/ru/python-net/aspose.cells/cells/unhide_rows/#int-int-float) | Отображает скрытые строки.|
| [set_row_height_pixel(row, pixels)](/cells/ru/python-net/aspose.cells/cells/set_row_height_pixel/#int-int) | Задает высоту строки в пикселях.|
| [set_row_height_inch(row, inches)](/cells/ru/python-net/aspose.cells/cells/set_row_height_inch/#int-float) | Устанавливает высоту строки в дюймах.|
| [set_row_height(row, height)](/cells/ru/python-net/aspose.cells/cells/set_row_height/#int-float) | Устанавливает высоту указанной строки.|
| [get_row_original_height_point(row)](/cells/ru/python-net/aspose.cells/cells/get_row_original_height_point/#int) | Получает высоту исходной строки в пунктах, если строка скрыта|
| [hide_column(column)](/cells/ru/python-net/aspose.cells/cells/hide_column/#int) | Скрывает столбец.|
| [unhide_column(column, width)](/cells/ru/python-net/aspose.cells/cells/unhide_column/#int-float) | Показать столбец|
| [hide_columns(column, total_columns)](/cells/ru/python-net/aspose.cells/cells/hide_columns/#int-int) | Скрыть несколько столбцов.|
| [unhide_columns(column, total_columns, width)](/cells/ru/python-net/aspose.cells/cells/unhide_columns/#int-int-float) |Показать несколько столбцов.|
| [get_row_height(row)](/cells/ru/python-net/aspose.cells/cells/get_row_height/#int) | Получает высоту указанной строки.|
| [get_view_row_height(row)](/cells/ru/python-net/aspose.cells/cells/get_view_row_height/#int) | Получает высоту указанной строки.|
| [get_row_height_pixel(row)](/cells/ru/python-net/aspose.cells/cells/get_row_height_pixel/#int) | Получает высоту указанной строки в пикселях.|
| [get_row_height_inch(row)](/cells/ru/python-net/aspose.cells/cells/get_row_height_inch/#int) | Получает высоту указанной строки в дюймах.|
| [get_view_row_height_inch(row)](/cells/ru/python-net/aspose.cells/cells/get_view_row_height_inch/#int) | Получает высоту указанной строки в дюймах.|
| [set_column_width_pixel(column, pixels)](/cells/ru/python-net/aspose.cells/cells/set_column_width_pixel/#int-int) | Задает ширину столбца в пикселях в обычном режиме просмотра.|
| [set_column_width_inch(column, inches)](/cells/ru/python-net/aspose.cells/cells/set_column_width_inch/#int-float) | Устанавливает ширину столбца в дюймах в обычном режиме просмотра.|
| [set_column_width(column, width)](/cells/ru/python-net/aspose.cells/cells/set_column_width/#int-float) | Задает ширину указанного столбца в обычном представлении.|
| [get_column_width_pixel(column)](/cells/ru/python-net/aspose.cells/cells/get_column_width_pixel/#int) | Получает ширину указанного столбца в обычном представлении в пикселях.|
| [get_column_width_inch(column)](/cells/ru/python-net/aspose.cells/cells/get_column_width_inch/#int) | Получает ширину указанного столбца в обычном представлении в дюймах.|
| [get_column_width(column)](/cells/ru/python-net/aspose.cells/cells/get_column_width/#int) | Получает ширину указанного столбца в обычном режиме|
| [get_view_column_width_pixel(column)](/cells/ru/python-net/aspose.cells/cells/get_view_column_width_pixel/#int) | Получите ширину в разных типах представления.|
| [set_view_column_width_pixel(column, pixels)](/cells/ru/python-net/aspose.cells/cells/set_view_column_width_pixel/#int-int) | Устанавливает ширину столбца в разных представлениях.|
| [get_last_data_row(column)](/cells/ru/python-net/aspose.cells/cells/get_last_data_row/#int) | Получает индекс последней строки ячейки, которая содержит данные в указанном столбце.|
| [apply_column_style(column, style, flag)](/cells/ru/python-net/aspose.cells/cells/apply_column_style/#int-Style-StyleFlag) | Применяет форматы ко всему столбцу.|
| [apply_row_style(row, style, flag)](/cells/ru/python-net/aspose.cells/cells/apply_row_style/#int-Style-StyleFlag) | Применяет форматы ко всей строке.|
| [apply_style(style, flag)](/cells/ru/python-net/aspose.cells/cells/apply_style/#Style-StyleFlag) | Применяет форматы ко всему рабочему листу.|
| [copy_column(source_cells, source_column_index, destination_column_index)](/cells/ru/python-net/aspose.cells/cells/copy_column/#Cells-int-int) | Копирует данные и форматы всего столбца.|
| [copy_row(source_cells, source_row_index, destination_row_index)](/cells/ru/python-net/aspose.cells/cells/copy_row/#Cells-int-int) | Копирует данные и форматы всей строки.|
| [get_grouped_row_outline_level(row_index)](/cells/ru/python-net/aspose.cells/cells/get_grouped_row_outline_level/#int) |Получает уровень структуры (отсчитываемый от нуля) строки.|
| [get_grouped_column_outline_level(column_index)](/cells/ru/python-net/aspose.cells/cells/get_grouped_column_outline_level/#int) | Получает уровень структуры (отсчитываемый от нуля) столбца.|
| [get_max_grouped_column_outline_level()](/cells/ru/python-net/aspose.cells/cells/get_max_grouped_column_outline_level/#) | Получает максимальный уровень структуры сгруппированного столбца (отсчитывается от нуля).|
| [get_max_grouped_row_outline_level()](/cells/ru/python-net/aspose.cells/cells/get_max_grouped_row_outline_level/#) | Получает максимальный уровень структуры сгруппированной строки (отсчитывается от нуля).|
| [show_group_detail(is_vertical, index)](/cells/ru/python-net/aspose.cells/cells/show_group_detail/#bool-int) | Разворачивает сгруппированные строки/столбцы.|
| [hide_group_detail(is_vertical, index)](/cells/ru/python-net/aspose.cells/cells/hide_group_detail/#bool-int) | Сворачивает сгруппированные строки/столбцы.|
| [ungroup_columns(first_index, last_index)](/cells/ru/python-net/aspose.cells/cells/ungroup_columns/#int-int) | Разгруппирует столбцы.|
| [delete_columns(column_index, total_columns, update_reference)](/cells/ru/python-net/aspose.cells/cells/delete_columns/#int-int-bool) | Удаляет несколько столбцов.|
| [is_deleting_range_enabled(start_row, start_column, total_rows, total_columns)](/cells/ru/python-net/aspose.cells/cells/is_deleting_range_enabled/#int-int-int-int) | Проверьте, можно ли удалить диапазон.|
| [delete_row(row_index)](/cells/ru/python-net/aspose.cells/cells/delete_row/#int) | Удаляет строку.|
| [is_blank_column(column_index)](/cells/ru/python-net/aspose.cells/cells/is_blank_column/#int) | Проверяет, является ли данный столбец пустым (не содержит данных).|
| [insert_row(row_index)](/cells/ru/python-net/aspose.cells/cells/insert_row/#int) | Вставляет новую строку в рабочий лист.|
| [link_to_xml_map(map_name, row, column, path)](/cells/ru/python-net/aspose.cells/cells/link_to_xml_map/#str-int-int-str) | Ссылка на xml-карту.|
| [find_formula(formula, previous_cell)](/cells/ru/python-net/aspose.cells/cells/find_formula/#str-Cell) | Находит ячейку с входной строкой.|
| [find_formula_contains(formula, previous_cell)](/cells/ru/python-net/aspose.cells/cells/find_formula_contains/#str-Cell) | Находит ячейку с формулой, содержащей введенную строку.|
| [move_range(source_area, dest_row, dest_column)](/cells/ru/python-net/aspose.cells/cells/move_range/#CellArea-int-int) | Перемещает диапазон.|
| [insert_cut_cells(cut_range, row, column, shift_type)](/cells/ru/python-net/aspose.cells/cells/insert_cut_cells/#Range-int-int-ShiftType) | Вставьте диапазон обрезки.|
| [delete_range(start_row, start_column, end_row, end_column, shift_type)](/cells/ru/python-net/aspose.cells/cells/delete_range/#int-int-int-int-ShiftType) | Удаляет диапазон ячеек и сдвигает ячейки в соответствии с параметром сдвига.|
| [retrieve_subtotal_setting(ca)](/cells/ru/python-net/aspose.cells/cells/retrieve_subtotal_setting/#CellArea) | Извлекает настройку промежуточных итогов диапазона.|
| [remove_formulas()](/cells/ru/python-net/aspose.cells/cells/remove_formulas/#) | Удаляет все формулы и заменяет значением формулы.|
| [convert_string_to_numeric_value()](/cells/ru/python-net/aspose.cells/cells/convert_string_to_numeric_value/#) |Преобразует строковые данные в ячейках в числовые значения, если это возможно.|
| [get_dependents(is_all, row, column)](/cells/ru/python-net/aspose.cells/cells/get_dependents/#bool-int-int) | Получить все ячейки, которые ссылаются на конкретную ячейку.|
| [get_dependents_in_calculation(row, column, recursive)](/cells/ru/python-net/aspose.cells/cells/get_dependents_in_calculation/#int-int-bool) | Получает все ячейки, вычисленный результат которых зависит от определенных ячеек.|
| [get_cell_style(row, column)](/cells/ru/python-net/aspose.cells/cells/get_cell_style/#int-int) | Получить стиль данной ячейки.|



###  Смотрите также
* модуль [aspose.cells](..)
* класс [Cell](/cells/ru/python-net/aspose.cells/cell)
* класс [Column](/cells/ru/python-net/aspose.cells/column)
* класс [Range](/cells/ru/python-net/aspose.cells/range)
* класс [Row](/cells/ru/python-net/aspose.cells/row)
