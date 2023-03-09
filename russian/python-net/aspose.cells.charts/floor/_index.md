---
title: Floor класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 160
url: /ru/python-net/aspose.cells.charts/floor/
is_root: false
---
##  Floor класс
Инкапсулирует объект, представляющий нижнюю часть трехмерной диаграммы.



**Наследование:** [Floor](/cells/python-net/aspose.cells.charts/floor) → 
[Area](/cells/ru/python-net/aspose.cells.drawing/area)



Тип Floor предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [background_color](/cells/ru/python-net/aspose.cells.charts/floor/background_color) | Получает или задает цвет фона объекта [Area](/cells/ru/python-net/aspose.cells.drawing/area).|
| [foreground_color](/cells/ru/python-net/aspose.cells.charts/floor/foreground_color) | Получает или задает цвет переднего плана.|
| [formatting](/cells/ru/python-net/aspose.cells.charts/floor/formatting) | Представляет форматирование области.|
| [invert_if_negative](/cells/ru/python-net/aspose.cells.charts/floor/invert_if_negative) | Если свойство истинно и значение точки диаграммы является отрицательным числом,<br/> цвет переднего плана и цвет фона будут заменены.|
| [fill_format](/cells/ru/python-net/aspose.cells.charts/floor/fill_format) | Представляет объект [Area.fill_format](/cells/ru/python-net/aspose.cells.drawing/area#fill_format), содержащий свойства форматирования заливки для указанной диаграммы или фигуры.|
| [transparency](/cells/ru/python-net/aspose.cells.charts/floor/transparency) | Возвращает или задает степень прозрачности области в виде значения от 0,0 (непрозрачная) до 1,0 (прозрачная).|
| [border](/cells/ru/python-net/aspose.cells.charts/floor/border) | Получает или задает границу [Line](/cells/ru/python-net/aspose.cells.drawing/line).|



###  Пример

```python
from aspose.cells import License, Workbook
from aspose.cells.charts import ChartType
from aspose.cells.drawing import GradientPresetType, GradientStyleType
from aspose.pydrawing import Color

# Instantiate the License class
license = License()
# Pass only the name of the license file embedded in the assembly
license.set_license("Aspose.Cells.lic")
# Instantiate the workbook object
workbook = Workbook()
# Get cells collection
cells = workbook.worksheets[0].cells
# Put values in cells
cells.get("A1").put_value(1)
cells.get("A2").put_value(2)
cells.get("A3").put_value(3)
# get charts colletion
charts = workbook.worksheets[0].charts
# add a new chart
index = charts.add(ChartType.COLUMN_3D_STACKED, 5, 0, 15, 5)
# get the newly added chart
chart = charts[index]
# set charts nseries
chart.n_series.add("A1:A3", True)
# Show data labels
chart.n_series[0].data_labels.show_value = True
# Get chart's floor
floor = chart.floor
# set floor's border as red
floor.border.color = Color.red
# set fill format
floor.fill_format.set_preset_color_gradient(GradientPresetType.CALM_WATER, GradientStyleType.DIAGONAL_DOWN, 2)
# save the file
workbook.save(r"dest.xls")

```

###  Смотрите также
* модуль [aspose.cells.charts](..)
* класс [Area](/cells/ru/python-net/aspose.cells.drawing/area)
* класс [Floor](/cells/ru/python-net/aspose.cells.charts/floor)
* класс [Line](/cells/ru/python-net/aspose.cells.drawing/line)
