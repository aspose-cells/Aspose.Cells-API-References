---
title: Line класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 290
url: /ru/python-net/aspose.cells.drawing/line/
is_root: false
---
##  Line класс
Инкапсулирует объект, представляющий формат строки.



Тип Line предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [compound_type](/cells/ru/python-net/aspose.cells.drawing/line/compound_type) |Задает тип составной линии|
| [dash_type](/cells/ru/python-net/aspose.cells.drawing/line/dash_type) | Указывает тип пунктирной линии|
| [cap_type](/cells/ru/python-net/aspose.cells.drawing/line/cap_type) | Определяет конечные заглавные буквы.|
| [join_type](/cells/ru/python-net/aspose.cells.drawing/line/join_type) | Определяет соединительные заглавные буквы.|
| [begin_type](/cells/ru/python-net/aspose.cells.drawing/line/begin_type) | Указывает стрелку для начала строки.|
| [end_type](/cells/ru/python-net/aspose.cells.drawing/line/end_type) | Задает стрелку для конца строки.|
| [begin_arrow_length](/cells/ru/python-net/aspose.cells.drawing/line/begin_arrow_length) | Определяет длину стрелки для начала строки.|
| [end_arrow_length](/cells/ru/python-net/aspose.cells.drawing/line/end_arrow_length) | Задает длину стрелки для конца строки.|
| [begin_arrow_width](/cells/ru/python-net/aspose.cells.drawing/line/begin_arrow_width) | Определяет ширину стрелки для начала строки.|
| [end_arrow_width](/cells/ru/python-net/aspose.cells.drawing/line/end_arrow_width) | Определяет ширину стрелки для конца строки.|
| [theme_color](/cells/ru/python-net/aspose.cells.drawing/line/theme_color) | Получает и задает цвет темы.|
| [color](/cells/ru/python-net/aspose.cells.drawing/line/color) | Представляет цвет линии.|
| [transparency](/cells/ru/python-net/aspose.cells.drawing/line/transparency) | Возвращает или задает степень прозрачности линии в виде значения от 0,0 (непрозрачная) до 1,0 (прозрачная).|
| [style](/cells/ru/python-net/aspose.cells.drawing/line/style) | Представляет стиль линии.|
| [weight](/cells/ru/python-net/aspose.cells.drawing/line/weight) | Получает или задает [WeightType](/cells/ru/python-net/aspose.cells.drawing/weighttype) строки.|
| [weight_pt](/cells/ru/python-net/aspose.cells.drawing/line/weight_pt) | Получает или задает вес линии в пунктах.|
| [weight_px](/cells/ru/python-net/aspose.cells.drawing/line/weight_px) | Получает или задает вес линии в пикселях.|
| [formatting_type](/cells/ru/python-net/aspose.cells.drawing/line/formatting_type) | Получает или задает тип формата.|
| [is_automatic_color](/cells/ru/python-net/aspose.cells.drawing/line/is_automatic_color) |Указывает, назначается ли цвет линии автоматически.|
| [is_visible](/cells/ru/python-net/aspose.cells.drawing/line/is_visible) | Указывает, видна ли линия.|
| [is_auto](/cells/ru/python-net/aspose.cells.drawing/line/is_auto) | Указывает, назначается ли этот стиль линии автоматически.|
| [gradient_fill](/cells/ru/python-net/aspose.cells.drawing/line/gradient_fill) | Представляет градиентную заливку.|



###  Пример

```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartMarkerType, ChartType
from aspose.cells.drawing import LineType, WeightType
from aspose.pydrawing import Color

workbook = Workbook()
sheet = workbook.worksheets[0]
cells = sheet.cells
cells.get(0, 1).put_value("Income")
cells.get(1, 0).put_value("Company A")
cells.get(2, 0).put_value("Company B")
cells.get(3, 0).put_value("Company C")
cells.get(1, 1).put_value(10000)
cells.get(2, 1).put_value(20000)
cells.get(3, 1).put_value(30000)
chartIndex = sheet.charts.add(ChartType.LINE, 9, 9, 21, 15)
chart = sheet.charts[chartIndex]
# Applying a dotted line style on the lines of an NSeries
chart.n_series[0].border.style = LineType.DOT
chart.n_series[0].border.color = Color.red
# Applying a triangular marker style on the data markers of an NSeries
chart.n_series[0].marker.marker_style = ChartMarkerType.TRIANGLE
# Setting the weight of all lines in an NSeries to medium
chart.n_series[0].border.weight = WeightType.MEDIUM_LINE

```

###  Смотрите также
* модуль [aspose.cells.drawing](..)
* класс [WeightType](/cells/ru/python-net/aspose.cells.drawing/weighttype)
