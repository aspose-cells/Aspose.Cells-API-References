---
title: ChartArea класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 40
url: /ru/python-net/aspose.cells.charts/chartarea/
is_root: false
---
##  ChartArea класс
Инкапсулирует объект, представляющий область диаграммы на листе.



**Наследование:** [ChartArea](/cells/python-net/aspose.cells.charts/chartarea) → 
[ChartFrame](/cells/ru/python-net/aspose.cells.charts/chartframe)



Тип ChartArea предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [is_inner_mode](/cells/ru/python-net/aspose.cells.charts/chartarea/is_inner_mode) | Указывает, включает ли размер области графика деления и метки осей.<br/> False указывает, что размер должен определять размер области графика, делений и меток осей.|
| [border](/cells/ru/python-net/aspose.cells.charts/chartarea/border) | Получает [Line](/cells/ru/python-net/aspose.cells.drawing/line).|
| [area](/cells/ru/python-net/aspose.cells.charts/chartarea/area) | Получает [ChartFrame.area](/cells/ru/python-net/aspose.cells.charts/chartframe#area).|
| [text_font](/cells/ru/python-net/aspose.cells.charts/chartarea/text_font) | Получает объект [ChartFrame.font](/cells/ru/python-net/aspose.cells.charts/chartframe#font) указанного объекта ChartFrame.|
| [text_options](/cells/ru/python-net/aspose.cells.charts/chartarea/text_options) | Получает и задает параметры текста.|
| [font](/cells/ru/python-net/aspose.cells.charts/chartarea/font) | Получает объект [ChartArea.font](/cells/ru/python-net/aspose.cells.charts/chartarea#font) указанного объекта диаграммы.|
| [auto_scale_font](/cells/ru/python-net/aspose.cells.charts/chartarea/auto_scale_font) | Истинно, если текст в объекте изменяет размер шрифта при изменении размера объекта. Значение по умолчанию верно.|
| [background_mode](/cells/ru/python-net/aspose.cells.charts/chartarea/background_mode) | Получает и задает режим отображения фона|
| [background](/cells/ru/python-net/aspose.cells.charts/chartarea/background) | Получает и задает режим отображения фона|
| [is_automatic_size](/cells/ru/python-net/aspose.cells.charts/chartarea/is_automatic_size) | Указывает, имеет ли рамка диаграммы автоматический размер.|
| [x](/cells/ru/python-net/aspose.cells.charts/chartarea/x) | Получает или получает горизонтальное смещение от верхнего левого углового столбца.|
| [y](/cells/ru/python-net/aspose.cells.charts/chartarea/y) |Получает или получает вертикальное смещение от строки верхнего левого угла.|
| [height](/cells/ru/python-net/aspose.cells.charts/chartarea/height) | Получает или задает вертикальное смещение от нижнего правого углового ряда.|
| [width](/cells/ru/python-net/aspose.cells.charts/chartarea/width) | Получает или задает смещение по горизонтали от нижнего правого углового столбца.|
| [shadow](/cells/ru/python-net/aspose.cells.charts/chartarea/shadow) | Истинно, если у кадра есть тень.|
| [shape_properties](/cells/ru/python-net/aspose.cells.charts/chartarea/shape_properties) | Получает объект [ChartFrame.shape_properties](/cells/ru/python-net/aspose.cells.charts/chartframe#shape_properties).|
| [is_default_pos_be_set](/cells/ru/python-net/aspose.cells.charts/chartarea/is_default_pos_be_set) | Указывает, задана ли позиция по умолчанию (DefaultX, DefaultY, DefaultWidth и DefaultHeight).|
| [default_x](/cells/ru/python-net/aspose.cells.charts/chartarea/default_x) | Представляет x позиции по умолчанию|
| [default_y](/cells/ru/python-net/aspose.cells.charts/chartarea/default_y) | Представляет y положения по умолчанию|
| [default_width](/cells/ru/python-net/aspose.cells.charts/chartarea/default_width) | Представляет ширину положения по умолчанию|
| [default_height](/cells/ru/python-net/aspose.cells.charts/chartarea/default_height) | Представляет высоту позиции по умолчанию|


###  Методы
| Метод| Описание|
| :- | :- |
| [set_position_auto()](/cells/ru/python-net/aspose.cells.charts/chartarea/set_position_auto/#) | Установите положение кадра на автоматический|



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
chartIndex = worksheet.charts.add(ChartType.COLUMN, 5, 0, 15, 5)
# Accessing the instance of the newly added chart
chart = worksheet.charts[chartIndex]
# Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.n_series.add("A1:B3", True)
# Getting Chart Area
chartArea = chart.chart_area
# Setting the foreground color of the chart area
chartArea.area.foreground_color = Color.yellow
# Setting Chart Area Shadow
chartArea.shadow = True
# Saving the Excel file
workbook.save("book1.xls")

```

###  Смотрите также
* модуль [aspose.cells.charts](..)
* класс [ChartArea](/cells/ru/python-net/aspose.cells.charts/chartarea)
* класс [ChartFrame](/cells/ru/python-net/aspose.cells.charts/chartframe)
* класс [Line](/cells/ru/python-net/aspose.cells.drawing/line)
