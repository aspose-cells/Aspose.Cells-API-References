---
title: is_chart_data_changed метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 70
url: /ru/python-net/aspose.cells.charts/chart/is_chart_data_changed/
is_root: false
---
##  is_chart_data_changed() {#}
Определяет, изменился ли источник данных диаграммы.


###  Возвращает

Возвращает true, если диаграмма изменилась, в противном случае возвращает false


```python
def is_chart_data_changed(self):
    ...
```


###  Примечания

Этот метод обнаруживает изменения в источнике данных диаграммы перед преобразованием диаграммы в формат изображения.
При первом вызове Chart.toImage будут записаны исходные данные диаграммы (например, XValuesParseData, ValuesParseData).
Перед повторным вызовом метода Chart.toImage вызовите метод IsChartDataChanged, чтобы проверить, нуждается ли Chart в повторной визуализации.


###  Смотрите также
* модуль [aspose.cells.charts](../../)
* класс [Chart](/cells/ru/python-net/aspose.cells.charts/chart)
