---
title: Cell класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 140
url: /ru/python-net/aspose.cells/cell/
is_root: false
---
##  Cell класс
Инкапсулирует объект, представляющий одну ячейку книги.



Тип Cell предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [worksheet](/cells/ru/python-net/aspose.cells/cell/worksheet) | Получает родительский рабочий лист.|
| [date_time_value](/cells/ru/python-net/aspose.cells/cell/date_time_value) | Получает значение DateTime, содержащееся в ячейке.|
| [row](/cells/ru/python-net/aspose.cells/cell/row) | Получает номер строки (начиная с нуля) ячейки.|
| [column](/cells/ru/python-net/aspose.cells/cell/column) | Получает номер столбца (начиная с нуля) ячейки.|
| [is_formula](/cells/ru/python-net/aspose.cells/cell/is_formula) | Указывает, содержит ли указанная ячейка формулу.|
| [type](/cells/ru/python-net/aspose.cells/cell/type) | Представляет тип значения ячейки.|
| [name](/cells/ru/python-net/aspose.cells/cell/name) | Получает имя ячейки.|
| [is_error_value](/cells/ru/python-net/aspose.cells/cell/is_error_value) | Проверяет, является ли значение этой ячейки ошибкой.|
| [is_numeric_value](/cells/ru/python-net/aspose.cells/cell/is_numeric_value) | Указывает, является ли внутреннее значение этой ячейки числовым (int, double и datetime)|
| [string_value](/cells/ru/python-net/aspose.cells/cell/string_value) |Получает строковое значение, содержащееся в ячейке. Если тип этой ячейки — строка, верните само строковое значение.<br/>Для других типов ячеек будет возвращено форматированное строковое значение (отформатированное в соответствии с указанным стилем этой ячейки).<br/>Отформатированное значение ячейки совпадает с тем, что вы можете получить из Excel при копировании ячейки в виде текста (например,<br/> копирование ячейки в текстовый редактор или экспорт в csv).|
| [string_value_without_format](/cells/ru/python-net/aspose.cells/cell/string_value_without_format) | Получает значение ячейки в виде строки без какого-либо формата.|
| [number_category_type](/cells/ru/python-net/aspose.cells/cell/number_category_type) | Представляет тип категории числового форматирования этой ячейки.|
| [display_string_value](/cells/ru/python-net/aspose.cells/cell/display_string_value) | Получает отформатированное строковое значение этой ячейки по стилю отображения ячейки.|
| [int_value](/cells/ru/python-net/aspose.cells/cell/int_value) | Получает целочисленное значение, содержащееся в ячейке.|
| [double_value](/cells/ru/python-net/aspose.cells/cell/double_value) | Получает двойное значение, содержащееся в ячейке.|
| [float_value](/cells/ru/python-net/aspose.cells/cell/float_value) | Получает значение с плавающей запятой, содержащееся в ячейке.|
| [bool_value](/cells/ru/python-net/aspose.cells/cell/bool_value) | Получает логическое значение, содержащееся в ячейке.|
| [has_custom_style](/cells/ru/python-net/aspose.cells/cell/has_custom_style) | Указывает, имеет ли эта ячейка пользовательские настройки стиля (отличные от унаследованных по умолчанию).<br/> из соответствующей строки, столбца или книги).|
| [shared_style_index](/cells/ru/python-net/aspose.cells/cell/shared_style_index) | Получает индекс общего стиля ячейки в пуле стилей.|
| [formula](/cells/ru/python-net/aspose.cells/cell/formula) | Получает или задает формулу [Cell](/cells/ru/python-net/aspose.cells/cell).|
| [formula_local](/cells/ru/python-net/aspose.cells/cell/formula_local) | Получите формулу ячейки в формате локали.|
| [r1c1_formula](/cells/ru/python-net/aspose.cells/cell/r1c1_formula) | Получает или задает формулу R1C1 для [Cell](/cells/ru/python-net/aspose.cells/cell).|
| [contains_external_link](/cells/ru/python-net/aspose.cells/cell/contains_external_link) |Указывает, содержит ли эта ячейка внешнюю ссылку.<br/> Применяется только в том случае, если ячейка является ячейкой формулы.|
| [is_array_header](/cells/ru/python-net/aspose.cells/cell/is_array_header) | Указывает, что формула ячейки и формула массива<br/> и это первая ячейка массива.|
| [is_dynamic_array_formula](/cells/ru/python-net/aspose.cells/cell/is_dynamic_array_formula) | Указывает, является ли формула ячейки формулой динамического массива (true) или устаревшей формулой массива (false).|
| [is_array_formula](/cells/ru/python-net/aspose.cells/cell/is_array_formula) | Указывает, является ли формула ячейки формулой массива.|
| [is_in_array](/cells/ru/python-net/aspose.cells/cell/is_in_array) | Указывает, является ли формула ячейки формулой массива.|
| [is_shared_formula](/cells/ru/python-net/aspose.cells/cell/is_shared_formula) | Указывает, является ли формула ячейки частью общей формулы.|
| [is_table_formula](/cells/ru/python-net/aspose.cells/cell/is_table_formula) | Указывает, является ли эта ячейка частью формулы таблицы.|
| [is_in_table](/cells/ru/python-net/aspose.cells/cell/is_in_table) | Указывает, является ли эта ячейка частью формулы таблицы.|
| [value](/cells/ru/python-net/aspose.cells/cell/value) | Получает значение, содержащееся в этой ячейке.|
| [is_style_set](/cells/ru/python-net/aspose.cells/cell/is_style_set) | Указывает, установлен ли стиль ячейки. Если возвращается false, это означает, что эта ячейка имеет формат ячейки по умолчанию.|
| [is_merged](/cells/ru/python-net/aspose.cells/cell/is_merged) | Проверяет, является ли ячейка частью объединенного диапазона или нет.|
| [comment](/cells/ru/python-net/aspose.cells/cell/comment) | Получает комментарий этой ячейки.|
| [html_string](/cells/ru/python-net/aspose.cells/cell/html_string) | Получает и задает строку html, содержащую данные и некоторые форматы в этой ячейке.|


###  Методы
| Метод| Описание|
| :- | :- |
| [calculate(options)](/cells/ru/python-net/aspose.cells/cell/calculate/#CalculationOptions) | Вычисляет формулу ячейки.|
| [calculate(ignore_error, custom_function)](/cells/ru/python-net/aspose.cells/cell/calculate/#bool-ICustomFunction) | Вычисляет формулу ячейки.|
| [put_value(bool_value)](/cells/ru/python-net/aspose.cells/cell/put_value/#bool) | Помещает логическое значение в ячейку.|
| [put_value(int_value)](/cells/ru/python-net/aspose.cells/cell/put_value/#int) | Помещает в ячейку целочисленное значение.|
| [put_value(double_value)](/cells/ru/python-net/aspose.cells/cell/put_value/#float) |Помещает двойное значение в ячейку.|
| [put_value(string_value, is_converted, set_style)](/cells/ru/python-net/aspose.cells/cell/put_value/#str-bool-bool) | Помещает значение в ячейку, при необходимости значение будет преобразовано в другой тип данных, а числовой формат ячейки будет сброшен.|
| [put_value(string_value, is_converted)](/cells/ru/python-net/aspose.cells/cell/put_value/#str-bool) | Помещает строковое значение в ячейку и при необходимости преобразует значение в другой тип данных.|
| [put_value(string_value)](/cells/ru/python-net/aspose.cells/cell/put_value/#str) | Помещает строковое значение в ячейку.|
| [put_value(date_time)](/cells/ru/python-net/aspose.cells/cell/put_value/#DateTime) | Помещает значение DateTime в ячейку.|
| [put_value(object_value)](/cells/ru/python-net/aspose.cells/cell/put_value/#any) | Помещает значение объекта в ячейку.|
| [get_display_style()](/cells/ru/python-net/aspose.cells/cell/get_display_style/#) | Получает стиль отображения ячейки.<br/>Если на эту ячейку также влияют другие параметры, такие как условное форматирование, объекты списка и т. д.,<br/> тогда стиль отображения может отличаться от cell.GetStyle().|
| [get_display_style(include_merged_borders)](/cells/ru/python-net/aspose.cells/cell/get_display_style/#bool) | Получает стиль отображения ячейки.<br/> Если ячейка имеет условное форматирование, стиль отображения отличается от стиля cell.GetStyle().|
| [get_style()](/cells/ru/python-net/aspose.cells/cell/get_style/#) | Получает стиль ячейки.|
| [get_style(check_borders)](/cells/ru/python-net/aspose.cells/cell/get_style/#bool) | Если checkBorders имеет значение true, проверьте, повлияют ли границы других ячеек на стиль этой ячейки.|
| [set_style(style)](/cells/ru/python-net/aspose.cells/cell/set_style/#Style) | Задает стиль ячейки.|
| [set_style(style, explicit_flag)](/cells/ru/python-net/aspose.cells/cell/set_style/#Style-bool) | Примените стиль ячейки.|
| [set_style(style, flag)](/cells/ru/python-net/aspose.cells/cell/set_style/#Style-StyleFlag) | Примените стиль ячейки.|
| [set_formula(formula, value)](/cells/ru/python-net/aspose.cells/cell/set_formula/#str-any) | Установите формулу и значение формулы.|
| [set_formula(formula, is_r1c1, is_local, value)](/cells/ru/python-net/aspose.cells/cell/set_formula/#str-bool-bool-any) | Установите формулу и значение формулы.|
| [set_formula(formula, options, value)](/cells/ru/python-net/aspose.cells/cell/set_formula/#str-FormulaParseOptions-any) | Установите формулу и значение формулы.|
| [set_array_formula(array_formula, row_number, column_number, is_r1c1, is_local)](/cells/ru/python-net/aspose.cells/cell/set_array_formula/#str-int-int-bool-bool) | Задает формулу массива для диапазона ячеек.|
| [set_array_formula(array_formula, row_number, column_number)](/cells/ru/python-net/aspose.cells/cell/set_array_formula/#str-int-int) |Задает формулу массива (устаревшая формула массива, введенная с помощью CTRL+SHIFT+ENTER в MS Excel) для диапазона ячеек.|
| [set_array_formula(array_formula, row_number, column_number, options)](/cells/ru/python-net/aspose.cells/cell/set_array_formula/#str-int-int-FormulaParseOptions) | Задает формулу массива для диапазона ячеек.|
| [set_array_formula(array_formula, row_number, column_number, options, values)](/cells/ru/python-net/aspose.cells/cell/set_array_formula/#str-int-int-FormulaParseOptions-list) | Задает формулу массива для диапазона ячеек.|
| [set_shared_formula(shared_formula, row_number, column_number, is_r1c1, is_local)](/cells/ru/python-net/aspose.cells/cell/set_shared_formula/#str-int-int-bool-bool) | Устанавливает формулу в диапазон ячеек.|
| [set_shared_formula(shared_formula, row_number, column_number)](/cells/ru/python-net/aspose.cells/cell/set_shared_formula/#str-int-int) | Задает общие формулы для диапазона ячеек.|
| [set_shared_formula(shared_formula, row_number, column_number, options)](/cells/ru/python-net/aspose.cells/cell/set_shared_formula/#str-int-int-FormulaParseOptions) | Задает общие формулы для диапазона ячеек.|
| [set_shared_formula(shared_formula, row_number, column_number, options, values)](/cells/ru/python-net/aspose.cells/cell/set_shared_formula/#str-int-int-FormulaParseOptions-list) | Задает общие формулы для диапазона ячеек.|
| [get_leafs()](/cells/ru/python-net/aspose.cells/cell/get_leafs/#) | Получите все ячейки, которые ссылаются на эту ячейку напрямую и должны быть обновлены при изменении этой ячейки.|
| [get_leafs(recursive)](/cells/ru/python-net/aspose.cells/cell/get_leafs/#bool) | Получить все ячейки, которые будут обновлены при изменении этой ячейки.|
| [set_dynamic_array_formula(array_formula, options, calculate_value)](/cells/ru/python-net/aspose.cells/cell/set_dynamic_array_formula/#str-FormulaParseOptions-bool) | Задает формулу динамического массива и по возможности распространяет формулу на соседние ячейки.|
| [set_dynamic_array_formula(array_formula, options, values, calculate_range, calculate_value)](/cells/ru/python-net/aspose.cells/cell/set_dynamic_array_formula/#str-FormulaParseOptions-list-bool-bool) | Задает формулу динамического массива и по возможности распространяет формулу на соседние ячейки.|
| [set_dynamic_array_formula(array_formula, options, values, calculate_range, calculate_value, copts)](/cells/ru/python-net/aspose.cells/cell/set_dynamic_array_formula/#str-FormulaParseOptions-list-bool-bool-CalculationOptions) | Задает формулу динамического массива и по возможности распространяет формулу на соседние ячейки.|
| [set_table_formula(row_number, column_number, row_input_cell, column_input_cell, values)](/cells/ru/python-net/aspose.cells/cell/set_table_formula/#int-int-str-str-list) | Создайте таблицу данных с двумя переменными для заданного диапазона, начиная с этой ячейки.|
| [set_table_formula(row_number, column_number, input_cell, is_row_input, values)](/cells/ru/python-net/aspose.cells/cell/set_table_formula/#int-int-str-bool-list) | Создайте таблицу данных с одной переменной для заданного диапазона, начиная с этой ячейки.|
| [set_table_formula(row_number, column_number, row_index_of_row_input_cell, column_index_of_row_input_cell, row_index_of_column_input_cell, column_index_of_column_input_cell, values)](/cells/ru/python-net/aspose.cells/cell/set_table_formula/#int-int-int-int-int-int-list) | Создайте таблицу данных с двумя переменными для заданного диапазона, начиная с этой ячейки.|
| [set_table_formula(row_number, column_number, row_index_of_input_cell, column_index_of_input_cell, is_row_input, values)](/cells/ru/python-net/aspose.cells/cell/set_table_formula/#int-int-int-int-bool-list) | Создайте таблицу данных с одной переменной для заданного диапазона, начиная с этой ячейки.|
| [get_characters()](/cells/ru/python-net/aspose.cells/cell/get_characters/#) | Возвращает все объекты символов<br/> который представляет собой диапазон символов в тексте ячейки.|
| [get_characters(flag)](/cells/ru/python-net/aspose.cells/cell/get_characters/#bool) | Возвращает все объекты символов<br/> который представляет собой диапазон символов в тексте ячейки.|
| [get_string_value(format_strategy)](/cells/ru/python-net/aspose.cells/cell/get_string_value/#CellValueFormatStrategy) | Получает строковое значение по определенной стратегии форматирования.|
| [get_width_of_value()](/cells/ru/python-net/aspose.cells/cell/get_width_of_value/#) | Получает ширину значения в пикселях.|
| [get_height_of_value()](/cells/ru/python-net/aspose.cells/cell/get_height_of_value/#) | Получает высоту значения в единицах пикселей.|
| [get_format_conditions()](/cells/ru/python-net/aspose.cells/cell/get_format_conditions/#) | Получает условия формата, применимые к этой ячейке.|
| [get_formula(is_r1c1, is_local)](/cells/ru/python-net/aspose.cells/cell/get_formula/#bool-bool) | Получите формулу этой ячейки.|
| [get_precedents()](/cells/ru/python-net/aspose.cells/cell/get_precedents/#) |Получает все ссылки, встречающиеся в формуле этой ячейки.|
| [get_dependents(is_all)](/cells/ru/python-net/aspose.cells/cell/get_dependents/#bool) | Получить все ячейки, формула которых напрямую ссылается на эту ячейку.|
| [get_precedents_in_calculation()](/cells/ru/python-net/aspose.cells/cell/get_precedents_in_calculation/#) | Получает все прецеденты (ссылки на ячейки в текущей книге), используемые формулой этой ячейки при ее вычислении.|
| [get_dependents_in_calculation(recursive)](/cells/ru/python-net/aspose.cells/cell/get_dependents_in_calculation/#bool) | Получает все ячейки, результат вычислений которых зависит от этой ячейки.|
| [get_array_range()](/cells/ru/python-net/aspose.cells/cell/get_array_range/#) | Получает диапазон массива, если формула ячейки является формулой массива.|
| [remove_array_formula(leave_normal_formula)](/cells/ru/python-net/aspose.cells/cell/remove_array_formula/#bool) | Удалить формулу массива.|
| [copy(cell)](/cells/ru/python-net/aspose.cells/cell/copy/#Cell) | Копирует данные из исходной ячейки.|
| [characters(start_index, length)](/cells/ru/python-net/aspose.cells/cell/characters/#int-int) | Возвращает объект Characters, представляющий диапазон символов в тексте ячейки.|
| [is_rich_text()](/cells/ru/python-net/aspose.cells/cell/is_rich_text/#) | Указывает, является ли значение строки ячейки форматированным текстом.|
| [set_characters(characters)](/cells/ru/python-net/aspose.cells/cell/set_characters/#list) | Устанавливает расширенный текстовый формат ячейки.|
| [get_merged_range()](/cells/ru/python-net/aspose.cells/cell/get_merged_range/#) | Возвращает объект [Range](/cells/ru/python-net/aspose.cells/range), представляющий объединенный диапазон.|
| [get_html_string(html5)](/cells/ru/python-net/aspose.cells/cell/get_html_string/#bool) | Получает строку html, содержащую данные и некоторые форматы в этой ячейке.|
| [to_json()](/cells/ru/python-net/aspose.cells/cell/to_json/#) | Преобразование [Cell](/cells/ru/python-net/aspose.cells/cell) в данные структуры JSON.|
| [equals(cell)](/cells/ru/python-net/aspose.cells/cell/equals/#Cell) | Проверяет, ссылается ли этот объект на ту же ячейку с другим объектом ячейки.|
| [get_conditional_formatting_result()](/cells/ru/python-net/aspose.cells/cell/get_conditional_formatting_result/#) | Получите результат условного форматирования.|
| [get_validation()](/cells/ru/python-net/aspose.cells/cell/get_validation/#) |Получает проверку, применяемую к этой ячейке.|
| [get_validation_value()](/cells/ru/python-net/aspose.cells/cell/get_validation_value/#) | Получает значение проверки, примененное к этой ячейке.|
| [get_table()](/cells/ru/python-net/aspose.cells/cell/get_table/#) | Получает таблицу, содержащую эту ячейку.|



###  Пример

```python
from aspose.cells import TextAlignmentType, Workbook
from aspose.pydrawing import Color

excel = Workbook()
cells = excel.worksheets[0].cells
# Put a string into a cell
cell = cells.get(0, 0)
cell.put_value("Hello")
first = cell.string_value
# Put an integer into a cell
cell = cells.get("B1")
cell.put_value(12)
second = cell.int_value
# Put a double into a cell
cell = cells.get(0, 2)
cell.put_value(-1.234)
third = cell.double_value
# Put a formula into a cell
cell = cells.get("D1")
cell.formula = "=B1 + C1"
# Put a combined formula: "sum(average(b1,c1), b1)" to cell at b2
cell = cells.get("b2")
cell.formula = "=sum(average(b1,c1), b1)"
# Set style of a cell
style = cell.get_style()
# Set background color
style.background_color = Color.yellow
# Set format of a cell
style.font.name = "Courier New"
style.vertical_alignment = TextAlignmentType.TOP
cell.set_style(style)

```

###  Смотрите также
* модуль [aspose.cells](..)
* класс [Cell](/cells/ru/python-net/aspose.cells/cell)
* класс [Range](/cells/ru/python-net/aspose.cells/range)
