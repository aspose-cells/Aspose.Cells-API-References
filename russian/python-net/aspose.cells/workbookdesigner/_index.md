---
title: WorkbookDesigner класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 1600
url: /ru/python-net/aspose.cells/workbookdesigner/
is_root: false
---
##  WorkbookDesigner класс
Инкапсулирует объект, представляющий электронную таблицу конструктора.



Тип WorkbookDesigner предоставляет следующие члены:

###  Конструкторы
| Конструктор| Описание|
| :- | :- |
| [WorkbookDesigner()](/cells/ru/python-net/aspose.cells/workbookdesigner/__init__/#) | Инициализирует новый экземпляр класса [WorkbookDesigner](/cells/ru/python-net/aspose.cells/workbookdesigner).|
| [WorkbookDesigner(workbook)](/cells/ru/python-net/aspose.cells/workbookdesigner/__init__/#Workbook) | Инициализирует новый экземпляр класса [WorkbookDesigner](/cells/ru/python-net/aspose.cells/workbookdesigner).|


###  Характеристики
| Свойство| Описание|
| :- | :- |
| [workbook](/cells/ru/python-net/aspose.cells/workbookdesigner/workbook) |Получает и задает объект [WorkbookDesigner.workbook](/cells/ru/python-net/aspose.cells/workbookdesigner#workbook).|
| [repeat_formulas_with_subtotal](/cells/ru/python-net/aspose.cells/workbookdesigner/repeat_formulas_with_subtotal) | Указывает, повторяются ли формулы со строками промежуточных итогов.|
| [update_empty_string_as_null](/cells/ru/python-net/aspose.cells/workbookdesigner/update_empty_string_as_null) | Если TRUE, Null будет вставлен, если значение равно "";|
| [update_reference](/cells/ru/python-net/aspose.cells/workbookdesigner/update_reference) |Указывает, будут ли обновлены ссылки на других рабочих листах.|
| [calculate_formula](/cells/ru/python-net/aspose.cells/workbookdesigner/calculate_formula) | Указывает, следует ли вычислять формулы.|
| [call_back](/cells/ru/python-net/aspose.cells/workbookdesigner/call_back) | Получает и задает интерфейс обратного вызова обработки смартмаркера.|
| [line_by_line](/cells/ru/python-net/aspose.cells/workbookdesigner/line_by_line) | Указывает, обрабатывается ли смарт-маркер построчно.|


###  Методы
| Метод| Описание|
| :- | :- |
| [set_data_source(data_source, cells_data_table)](/cells/ru/python-net/aspose.cells/workbookdesigner/set_data_source/#str-ICellsDataTable) | Устанавливает источник данных объекта [ICellsDataTable](/cells/ru/python-net/aspose.cells/icellsdatatable).|
| [set_data_source(variable, data)](/cells/ru/python-net/aspose.cells/workbookdesigner/set_data_source/#str-any) | Устанавливает привязку данных к переменной.|
| [process()](/cells/ru/python-net/aspose.cells/workbookdesigner/process/#) | Обрабатывает интеллектуальные маркеры и заполняет значения источника данных.|
| [process(is_preserved)](/cells/ru/python-net/aspose.cells/workbookdesigner/process/#bool) | Обрабатывает интеллектуальные маркеры и заполняет значения источника данных.|
| [process(sheet_index, is_preserved)](/cells/ru/python-net/aspose.cells/workbookdesigner/process/#int-bool) | Обрабатывает интеллектуальные маркеры и заполняет значения источника данных.|
| [clear_data_source()](/cells/ru/python-net/aspose.cells/workbookdesigner/clear_data_source/#) | Очищает все источники данных.|
| [get_smart_markers()](/cells/ru/python-net/aspose.cells/workbookdesigner/get_smart_markers/#) | Возвращает набор интеллектуальных маркеров в электронной таблице.|



###  Примеры

```python
from aspose.cells import Workbook, WorkbookDesigner

# Create WorkbookDesigner object.
wd = WorkbookDesigner()
# Open the template file (which contains smart markers).
wd.workbook = Workbook("SmartMarker_Designer.xls")
# Initialize your data from data source
# DataSet ds = new DataSet();
# ...
# Set the datatable as the data source.
# wd.SetDataSource(dt);
# Process the smart markers to fill the data into the worksheets.
wd.process(True)
# Save the excel file.
wd.workbook.save("outSmartMarker_Designer.xls")

```

###  Смотрите также
* модуль [aspose.cells](..)
* класс [ICellsDataTable](/cells/ru/python-net/aspose.cells/icellsdatatable)
* класс [WorkbookDesigner](/cells/ru/python-net/aspose.cells/workbookdesigner)
