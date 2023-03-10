---
title: FillFormat класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 180
url: /ru/python-net/aspose.cells.drawing/fillformat/
is_root: false
---
##  FillFormat класс
Инкапсулирует объект, представляющий форматирование заливки для фигуры.



Тип FillFormat предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [type](/cells/ru/python-net/aspose.cells.drawing/fillformat/type) |Получает и задает тип заполнения.|
| [fill_type](/cells/ru/python-net/aspose.cells.drawing/fillformat/fill_type) | Получает и задает тип заполнения|
| [transparency](/cells/ru/python-net/aspose.cells.drawing/fillformat/transparency) | Возвращает или задает степень прозрачности области в виде значения от 0,0 (непрозрачная) до 1,0 (прозрачная).|
| [set_type](/cells/ru/python-net/aspose.cells.drawing/fillformat/set_type) | Получает тип набора форматов заливки.|
| [gradient_fill](/cells/ru/python-net/aspose.cells.drawing/fillformat/gradient_fill) | Получает объект [FillFormat.gradient_fill](/cells/ru/python-net/aspose.cells.drawing/fillformat#gradient_fill).|
| [texture_fill](/cells/ru/python-net/aspose.cells.drawing/fillformat/texture_fill) | Получает объект [FillFormat.texture_fill](/cells/ru/python-net/aspose.cells.drawing/fillformat#texture_fill).|
| [solid_fill](/cells/ru/python-net/aspose.cells.drawing/fillformat/solid_fill) | Получает объект [FillFormat.solid_fill](/cells/ru/python-net/aspose.cells.drawing/fillformat#solid_fill).|
| [pattern_fill](/cells/ru/python-net/aspose.cells.drawing/fillformat/pattern_fill) | Получает объект [FillFormat.pattern_fill](/cells/ru/python-net/aspose.cells.drawing/fillformat#pattern_fill).|
| [gradient_color_type](/cells/ru/python-net/aspose.cells.drawing/fillformat/gradient_color_type) | Возвращает тип цвета градиента для указанной заливки.|
| [gradient_style](/cells/ru/python-net/aspose.cells.drawing/fillformat/gradient_style) | Возвращает стиль градиента для указанной заливки.|
| [gradient_color1](/cells/ru/python-net/aspose.cells.drawing/fillformat/gradient_color1) | Возвращает цвет градиента 1 для указанной заливки.|
| [gradient_color2](/cells/ru/python-net/aspose.cells.drawing/fillformat/gradient_color2) | Возвращает цвет градиента 2 для указанной заливки.|
| [gradient_degree](/cells/ru/python-net/aspose.cells.drawing/fillformat/gradient_degree) | Возвращает степень градиента для указанной заливки.<br/> Применяется только для Excel 2007.|
| [gradient_variant](/cells/ru/python-net/aspose.cells.drawing/fillformat/gradient_variant) | Возвращает вариант градиента для указанной заливки.<br/> Применяется только для Excel 2007.|
| [preset_color](/cells/ru/python-net/aspose.cells.drawing/fillformat/preset_color) | Возвращает заданный цвет градиента для указанной заливки.|
| [texture](/cells/ru/python-net/aspose.cells.drawing/fillformat/texture) | Представляет тип текстуры для указанной заливки.|
| [pattern](/cells/ru/python-net/aspose.cells.drawing/fillformat/pattern) | Представляет шаблон отображения области.|
| [picture_format_type](/cells/ru/python-net/aspose.cells.drawing/fillformat/picture_format_type) | Получает и задает тип формата изображения.|
| [scale](/cells/ru/python-net/aspose.cells.drawing/fillformat/scale) | Получает и задает масштаб формата изображения.|
| [image_data](/cells/ru/python-net/aspose.cells.drawing/fillformat/image_data) | Получает и задает данные изображения изображения.|


###  Методы
| Метод| Описание|
| :- | :- |
| [set_two_color_gradient(color1, color2, style, variant)](/cells/ru/python-net/aspose.cells.drawing/fillformat/set_two_color_gradient/#aspose.pydrawing.Color-aspose.pydrawing.Color-GradientStyleType-int) | Задает для указанной заливки двухцветный градиент.<br/> Применяется только для Excel 2007.|
| [set_two_color_gradient(color1, transparency1, color2, transparency2, style, variant)](/cells/ru/python-net/aspose.cells.drawing/fillformat/set_two_color_gradient/#aspose.pydrawing.Color-float-aspose.pydrawing.Color-float-GradientStyleType-int) | Задает для указанной заливки двухцветный градиент.<br/> Применяется только для Excel 2007.|
| [set_one_color_gradient(color, degree, style, variant)](/cells/ru/python-net/aspose.cells.drawing/fillformat/set_one_color_gradient/#aspose.pydrawing.Color-float-GradientStyleType-int) | Задает для указанной заливки одноцветный градиент.<br/> Применяется только для Excel 2007.|
| [set_preset_color_gradient(preset_color, style, variant)](/cells/ru/python-net/aspose.cells.drawing/fillformat/set_preset_color_gradient/#GradientPresetType-GradientStyleType-int) | Устанавливает для указанной заливки градиент предустановленного цвета.<br/> Применяется только для Excel 2007.|



###  Пример

```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartType
from aspose.cells.drawing import GradientStyleType
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
# Adding a new worksheet to the Excel object
sheetIndex = workbook.worksheets.add()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[sheetIndex]
# Adding a sample value to "A1" cell
worksheet.cells.get("A1").put_value(50)
# Adding a sample value to "A2" cell
worksheet.cells.get("A2").put_value(100)
# Adding a sample value to "A3" cell
worksheet.cells.get("A3").put_value(150)
# Adding a sample value to "A4" cell
worksheet.cells.get("A4").put_value(200)
# Adding a sample value to "B1" cell
worksheet.cells.get("B1").put_value(60)
# Adding a sample value to "B2" cell
worksheet.cells.get("B2").put_value(32)
# Adding a sample value to "B3" cell
worksheet.cells.get("B3").put_value(50)
# Adding a sample value to "B4" cell
worksheet.cells.get("B4").put_value(40)
# Adding a sample value to "C1" cell as category data
worksheet.cells.get("C1").put_value("Q1")
# Adding a sample value to "C2" cell as category data
worksheet.cells.get("C2").put_value("Q2")
# Adding a sample value to "C3" cell as category data
worksheet.cells.get("C3").put_value("Y1")
# Adding a sample value to "C4" cell as category data
worksheet.cells.get("C4").put_value("Y2")
# Adding a chart to the worksheet
chartIndex = worksheet.charts.add(ChartType.COLUMN, 5, 0, 15, 5)
# Accessing the instance of the newly added chart
chart = worksheet.charts[chartIndex]
# Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
seriesIndex = chart.n_series.add("A1:B4", True)
# Setting the data source for the category data of NSeries
chart.n_series.category_data = "C1:C4"
# Filling the area of the 2nd NSeries with a gradient
chart.n_series[seriesIndex].area.fill_format.set_one_color_gradient(Color.lime, 1, GradientStyleType.HORIZONTAL, 1)

```

###  Смотрите также
* модуль [aspose.cells.drawing](..)
