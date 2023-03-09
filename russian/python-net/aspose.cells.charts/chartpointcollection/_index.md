---
title: ChartPointCollection класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 100
url: /ru/python-net/aspose.cells.charts/chartpointcollection/
is_root: false
---
##  ChartPointCollection класс
Представляет коллекцию, содержащую все точки одной серии.



Тип ChartPointCollection предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [count](/cells/ru/python-net/aspose.cells.charts/chartpointcollection/count) | Получает количество точек диаграммы.|



Получает элемент [ChartPoint](/cells/ru/python-net/aspose.cells.charts/chartpoint) по указанному индексу в серии.
###  Индексатор
| Имя| Описание|
| :- | :- |
| [index] | Индекс точки графика в ряду.|


###  Методы
| Метод| Описание|
| :- | :- |
| [get_enumerator()](/cells/ru/python-net/aspose.cells.charts/chartpointcollection/get_enumerator/#) | Возвращает перечислитель для всего [ChartPointCollection](/cells/ru/python-net/aspose.cells.charts/chartpointcollection).|
| [clear()](/cells/ru/python-net/aspose.cells.charts/chartpointcollection/clear/#) | Удалите все настройки точек графика.|
| [remove_at(index)](/cells/ru/python-net/aspose.cells.charts/chartpointcollection/remove_at/#int) | Удаляет точку в индексе серии.|



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
chartIndex = worksheet.charts.add(ChartType.PIE_EXPLODED, 5, 0, 25, 10)
# Accessing the instance of the newly added chart
chart = worksheet.charts[chartIndex]
# Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.n_series.add("A1:B3", True)
# Show Data Labels
chart.n_series[0].data_labels.show_value = True
points = chart.n_series[0].points
for i in range(points.count):
    # Get Data Point
    point = points[i]
    # Set Pir Explosion
    point.explosion = 15
    # Set Border Color
    point.border.color = Color.red
# Saving the Excel file
workbook.save("book1.xls")

```

###  Смотрите также
* модуль [aspose.cells.charts](..)
* класс [ChartPoint](/cells/ru/python-net/aspose.cells.charts/chartpoint)
* класс [ChartPointCollection](/cells/ru/python-net/aspose.cells.charts/chartpointcollection)
