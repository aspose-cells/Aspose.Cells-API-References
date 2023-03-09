---
title: ChartPoint класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 90
url: /ru/python-net/aspose.cells.charts/chartpoint/
is_root: false
---
##  ChartPoint класс
Представляет одну точку в ряду на диаграмме.



Тип ChartPoint предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [explosion](/cells/ru/python-net/aspose.cells.charts/chartpoint/explosion) | Расстояние открытого сегмента круговой диаграммы от центра круговой диаграммы выражается в процентах от диаметра круговой диаграммы.|
| [shadow](/cells/ru/python-net/aspose.cells.charts/chartpoint/shadow) | Истинно, если точка диаграммы имеет тень.|
| [border](/cells/ru/python-net/aspose.cells.charts/chartpoint/border) | Получает [Line](/cells/ru/python-net/aspose.cells.drawing/line).|
| [area](/cells/ru/python-net/aspose.cells.charts/chartpoint/area) | Получает [ChartPoint.area](/cells/ru/python-net/aspose.cells.charts/chartpoint#area).|
| [marker](/cells/ru/python-net/aspose.cells.charts/chartpoint/marker) | Получает [ChartPoint.marker](/cells/ru/python-net/aspose.cells.charts/chartpoint#marker).|
| [data_labels](/cells/ru/python-net/aspose.cells.charts/chartpoint/data_labels) | Возвращает объект DataLabels, представляющий метку данных, связанную с точкой.|
| [y_value](/cells/ru/python-net/aspose.cells.charts/chartpoint/y_value) | Получает или задает значение Y точки диаграммы.|
| [y_value_type](/cells/ru/python-net/aspose.cells.charts/chartpoint/y_value_type) | Получает тип значения Y точки диаграммы.|
| [x_value](/cells/ru/python-net/aspose.cells.charts/chartpoint/x_value) |Получает или задает значение X точки диаграммы.|
| [x_value_type](/cells/ru/python-net/aspose.cells.charts/chartpoint/x_value_type) | Получает тип значения X точки диаграммы.|
| [shape_properties](/cells/ru/python-net/aspose.cells.charts/chartpoint/shape_properties) | Получает объект [ShapePropertyCollection](/cells/ru/python-net/aspose.cells.drawing/shapepropertycollection), содержащий свойства визуальной формы ChartPoint.|
| [is_in_secondary_plot](/cells/ru/python-net/aspose.cells.charts/chartpoint/is_in_secondary_plot) | Получает или задает значение, указывающее, находятся ли эти точки данных во второй круговой диаграмме или столбце.<br/> на круговой диаграмме или столбце круговой диаграммы|
| [shape_x](/cells/ru/python-net/aspose.cells.charts/chartpoint/shape_x) | Получает координату x левого верхнего угла в единицах 1/4000 ширины графика после вызова метода Chart.Calculate().|
| [shape_y](/cells/ru/python-net/aspose.cells.charts/chartpoint/shape_y) | Получает координату y левого верхнего угла в единицах 1/4000 высоты графика после вызова метода Chart.Calculate().|
| [shape_width](/cells/ru/python-net/aspose.cells.charts/chartpoint/shape_width) | Получает ширину в единицах 1/4000 ширины графика после вызова метода Chart.Calculate().|
| [shape_height](/cells/ru/python-net/aspose.cells.charts/chartpoint/shape_height) | Получает высоту в единицах 1/4000 высоты графика после вызова метода Chart.Calculate().|
| [shape_x_px](/cells/ru/python-net/aspose.cells.charts/chartpoint/shape_x_px) | Получает координату x левого верхнего угла в пикселях после вызова метода Chart.Calculate().|
| [shape_y_px](/cells/ru/python-net/aspose.cells.charts/chartpoint/shape_y_px) | Получает координату y верхнего левого угла в пикселях после вызова метода Chart.Calculate().|
| [shape_width_px](/cells/ru/python-net/aspose.cells.charts/chartpoint/shape_width_px) |Получает ширину в пикселях после вызова метода Chart.Calculate().|
| [shape_height_px](/cells/ru/python-net/aspose.cells.charts/chartpoint/shape_height_px) | Получает высоту в пикселях после вызова метода Chart.Calculate().|
| [border_width_px](/cells/ru/python-net/aspose.cells.charts/chartpoint/border_width_px) | Получает ширину границы в пикселях после вызова метода Chart.Calculate().|
| [radius_px](/cells/ru/python-net/aspose.cells.charts/chartpoint/radius_px) | Получает радиус пузырька, круга или пончика в пикселях после вызова метода Chart.Calculate().|
| [inner_radius_px](/cells/ru/python-net/aspose.cells.charts/chartpoint/inner_radius_px) | Получает внутренний радиус среза пончика в пикселях после вызова метода Chart.Calculate().<br/> Применяется к кольцевой диаграмме.|
| [start_angle](/cells/ru/python-net/aspose.cells.charts/chartpoint/start_angle) | Получает начальный угол для сегмента круговой диаграммы, измеренный в градусах по часовой стрелке от оси x после вызова метода Chart.Calculate().<br/> Применяется к круговой диаграмме.|
| [end_angle](/cells/ru/python-net/aspose.cells.charts/chartpoint/end_angle) | Получает конечный угол для сегмента круговой диаграммы, измеренный в градусах по часовой стрелке от оси x после вызова метода Chart.Calculate().<br/> Применяется к круговой диаграмме.|
| [arc_start_point_x_px](/cells/ru/python-net/aspose.cells.charts/chartpoint/arc_start_point_x_px) | Получает координату x начальной точки сектора круговой диаграммы после вызова метода Chart.Calculate().<br/> Применяется к круговой и кольцевой диаграммам.|
| [arc_start_point_y_px](/cells/ru/python-net/aspose.cells.charts/chartpoint/arc_start_point_y_px) |Получает координату y начальной точки сектора круга после вызова метода Chart.Calculate().<br/> Применяется к круговой и кольцевой диаграммам.|
| [arc_end_point_x_px](/cells/ru/python-net/aspose.cells.charts/chartpoint/arc_end_point_x_px) | Получает координату x конечной точки сектора круговой диаграммы после вызова метода Chart.Calculate().<br/> Применяется к круговой и кольцевой диаграммам.|
| [arc_end_point_y_px](/cells/ru/python-net/aspose.cells.charts/chartpoint/arc_end_point_y_px) | Получает координату y конечной точки сектора круга после вызова метода Chart.Calculate().<br/> Применяется к круговой и кольцевой диаграммам.|
| [inner_arc_start_point_x_px](/cells/ru/python-net/aspose.cells.charts/chartpoint/inner_arc_start_point_x_px) | Получает координату x начальной точки сектора круговой диаграммы после вызова метода Chart.Calculate().<br/> Применяется к кольцевой диаграмме.|
| [inner_arc_start_point_y_px](/cells/ru/python-net/aspose.cells.charts/chartpoint/inner_arc_start_point_y_px) |Получает координату y начальной точки сектора круга после вызова метода Chart.Calculate().<br/> Применяется к кольцевой диаграмме.|
| [inner_arc_end_point_x_px](/cells/ru/python-net/aspose.cells.charts/chartpoint/inner_arc_end_point_x_px) | Получает координату x конечной точки сектора круговой диаграммы после вызова метода Chart.Calculate().<br/> Применяется к кольцевой диаграмме.|
| [inner_arc_end_point_y_px](/cells/ru/python-net/aspose.cells.charts/chartpoint/inner_arc_end_point_y_px) | Получает координату y конечной точки сектора круга после вызова метода Chart.Calculate().<br/> Применяется к кольцевой диаграмме.|


###  Методы
| Метод| Описание|
| :- | :- |
| [get_top_point_count()](/cells/ru/python-net/aspose.cells.charts/chartpoint/get_top_point_count/#) | Получает количество верхних точек после вызова метода Chart.Calculate().|
| [get_top_point_x_px(index)](/cells/ru/python-net/aspose.cells.charts/chartpoint/get_top_point_x_px/#int) | Получает x-координату верхней точки фигуры после вызова метода Chart.Calculate().<br/> Применяет трехмерные диаграммы: Column3D, Bar3D, Cone, Cylinder, Pyramid и Area3D.|
| [get_top_point_y_px(index)](/cells/ru/python-net/aspose.cells.charts/chartpoint/get_top_point_y_px/#int) | Получает координату y верхней точки фигуры после вызова метода Chart.Calculate().<br/> Применяет трехмерные диаграммы: Column3D, Bar3D, Cone, Cylinder, Pyramid и Area3D.|
| [get_bottom_point_count()](/cells/ru/python-net/aspose.cells.charts/chartpoint/get_bottom_point_count/#) | Получает количество точек дна после вызова метода Chart.Calculate().|
| [get_bottom_point_x_px(index)](/cells/ru/python-net/aspose.cells.charts/chartpoint/get_bottom_point_x_px/#int) | Получает x-координату нижней точки фигуры после вызова метода Chart.Calculate().<br/> Применяет трехмерные диаграммы: Column3D, Bar3D, Cone, Cylinder, Pyramid|
| [get_bottom_point_y_px(index)](/cells/ru/python-net/aspose.cells.charts/chartpoint/get_bottom_point_y_px/#int) | Получает координату y нижней точки фигуры после вызова метода Chart.Calculate().<br/> Применяет трехмерные диаграммы: Column3D, Bar3D, Cone, Cylinder, Pyramid|
| [get_on_category_axis_point_count()](/cells/ru/python-net/aspose.cells.charts/chartpoint/get_on_category_axis_point_count/#) |Получает количество точек на оси категорий после вызова метода Chart.Calculate() Применяется только к диаграмме с областями.|
| [get_on_category_axis_point_x_px(index)](/cells/ru/python-net/aspose.cells.charts/chartpoint/get_on_category_axis_point_x_px/#int) | Получает x-координату точки на оси категорий после вызова метода Chart.Calculate() Применяется только к диаграмме с областями.|
| [get_on_category_axis_point_y_px(index)](/cells/ru/python-net/aspose.cells.charts/chartpoint/get_on_category_axis_point_y_px/#int) | Получает координату y точки на оси категорий после вызова метода Chart.Calculate() Применяется только к диаграмме с областями.|



###  Примеры

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
for i in range(chart.n_series[0].points.count):
    # Get Data Point
    point = chart.n_series[0].points[i]
    # Set Pir Explosion
    point.explosion = 15
    # Set Border Color
    point.border.color = Color.red
# Saving the Excel file
workbook.save("book1.xls")

```

###  Смотрите также
* модуль [aspose.cells.charts](..)
* класс [Line](/cells/ru/python-net/aspose.cells.drawing/line)
* класс [ShapePropertyCollection](/cells/ru/python-net/aspose.cells.drawing/shapepropertycollection)
