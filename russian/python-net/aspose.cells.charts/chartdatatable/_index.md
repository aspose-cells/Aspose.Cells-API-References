---
title: ChartDataTable класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 60
url: /ru/python-net/aspose.cells.charts/chartdatatable/
is_root: false
---
##  ChartDataTable класс
Представляет таблицу данных диаграммы.



Тип ChartDataTable предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [font](/cells/ru/python-net/aspose.cells.charts/chartdatatable/font) | Получает объект [ChartDataTable.font](/cells/ru/python-net/aspose.cells.charts/chartdatatable#font), представляющий настройку шрифта указанной таблицы данных диаграммы.|
| [auto_scale_font](/cells/ru/python-net/aspose.cells.charts/chartdatatable/auto_scale_font) | Истинно, если текст в объекте изменяет размер шрифта при изменении размера объекта.<br/> Значение по умолчанию верно.|
| [background_mode](/cells/ru/python-net/aspose.cells.charts/chartdatatable/background_mode) | Получает и задает режим отображения фона|
| [background](/cells/ru/python-net/aspose.cells.charts/chartdatatable/background) | Получает и задает режим отображения фона|
| [has_border_horizontal](/cells/ru/python-net/aspose.cells.charts/chartdatatable/has_border_horizontal) | Истинно, если таблица данных диаграммы имеет горизонтальные границы ячеек|
| [has_border_vertical](/cells/ru/python-net/aspose.cells.charts/chartdatatable/has_border_vertical) | Истинно, если таблица данных диаграммы имеет вертикальные границы ячеек|
| [has_border_outline](/cells/ru/python-net/aspose.cells.charts/chartdatatable/has_border_outline) | Истинно, если таблица данных диаграммы имеет контурные границы|
| [show_legend_key](/cells/ru/python-net/aspose.cells.charts/chartdatatable/show_legend_key) |Истинно, если ключ легенды метки данных виден.|
| [border](/cells/ru/python-net/aspose.cells.charts/chartdatatable/border) | Возвращает объект Border, представляющий границу объекта.|



###  Пример

```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartType
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the first worksheet
worksheet = workbook.worksheets[0]
# Adding a sample value to "A1" cell
worksheet.cells.get("A1").put_value(50)
# Adding a sample value to "A2" cell
worksheet.cells.get("A2").put_value(100)
# Adding a sample value to "A3" cell
worksheet.cells.get("A3").put_value(150)
# Adding a sample value to "B1" cell
worksheet.cells.get("B1").put_value(60)
# Adding a sample value to "B2" cell
worksheet.cells.get("B2").put_value(32)
# Adding a sample value to "B3" cell
worksheet.cells.get("B3").put_value(50)
# Adding a chart to the worksheet
chartIndex = worksheet.charts.add(ChartType.COLUMN, 5, 0, 25, 10)
# Accessing the instance of the newly added chart
chart = worksheet.charts[chartIndex]
# Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.n_series.add("A1:B3", True)
chart.show_data_table = True
# Getting Chart Table
chartTable = chart.chart_data_table
# Setting Chart Table Font Color
chartTable.font.color = Color.red
# Setting Legend Key VisibilityOptions
chartTable.show_legend_key = False
# Saving the Excel file
workbook.save("book1.xls")

```

###  Смотрите также
* модуль [aspose.cells.charts](..)
