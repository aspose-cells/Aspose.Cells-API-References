---
title: Floor sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 160
url: /tr/python-net/aspose.cells.charts/floor/
is_root: false
---
##  Floor sınıfı
3 boyutlu grafiğin zeminini temsil eden nesneyi kapsüller.



**Miras:** [Floor](/cells/python-net/aspose.cells.charts/floor) → 
[Area](/cells/tr/python-net/aspose.cells.drawing/area)



Floor türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [background_color](/cells/tr/python-net/aspose.cells.charts/floor/background_color) | [Area](/cells/tr/python-net/aspose.cells.drawing/area)'in arka plan rengini alır veya ayarlar.|
| [foreground_color](/cells/tr/python-net/aspose.cells.charts/floor/foreground_color) | Ön plan Rengini alır veya ayarlar.|
| [formatting](/cells/tr/python-net/aspose.cells.charts/floor/formatting) | Alanın biçimlendirmesini temsil eder.|
| [invert_if_negative](/cells/tr/python-net/aspose.cells.charts/floor/invert_if_negative) | Özellik true ise ve grafik noktasının değeri negatif bir sayıysa,<br/> ön plan rengi ve arka plan rengi değiştirilecektir.|
| [fill_format](/cells/tr/python-net/aspose.cells.charts/floor/fill_format) | Belirtilen grafik veya şekil için dolgu biçimlendirme özelliklerini içeren bir [Area.fill_format](/cells/tr/python-net/aspose.cells.drawing/area#fill_format) nesnesini temsil eder.|
| [transparency](/cells/tr/python-net/aspose.cells.charts/floor/transparency) | Alanın şeffaflık derecesini 0,0 (opak) ila 1,0 (temiz) arasında bir değer olarak döndürür veya ayarlar.|
| [border](/cells/tr/python-net/aspose.cells.charts/floor/border) | [Line](/cells/tr/python-net/aspose.cells.drawing/line) kenarlığını alır veya ayarlar.|



###  örnekler

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

###  Ayrıca bakınız
* modül [aspose.cells.charts](..)
* sınıf [Area](/cells/tr/python-net/aspose.cells.drawing/area)
* sınıf [Floor](/cells/tr/python-net/aspose.cells.charts/floor)
* sınıf [Line](/cells/tr/python-net/aspose.cells.drawing/line)
