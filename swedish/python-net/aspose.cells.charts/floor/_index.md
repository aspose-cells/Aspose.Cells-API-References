---
title: Floor klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 160
url: /sv/python-net/aspose.cells.charts/floor/
is_root: false
---
##  Floor klass
Kapslar in objektet som representerar golvet i ett 3D-diagram.



**Arv:** [Floor](/cells/python-net/aspose.cells.charts/floor) → 
[Area](/cells/sv/python-net/aspose.cells.drawing/area)



Typen Floor avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [background_color](/cells/sv/python-net/aspose.cells.charts/floor/background_color) | Hämtar eller ställer in bakgrundsfärgen för [Area](/cells/sv/python-net/aspose.cells.drawing/area).|
| [foreground_color](/cells/sv/python-net/aspose.cells.charts/floor/foreground_color) | Får eller ställer in förgrundsfärgen.|
| [formatting](/cells/sv/python-net/aspose.cells.charts/floor/formatting) | Representerar formateringen av området.|
| [invert_if_negative](/cells/sv/python-net/aspose.cells.charts/floor/invert_if_negative) | Om egenskapen är sann och värdet på diagrampunkten är ett negativt tal,<br/> förgrundsfärgen och bakgrundsfärgen kommer att bytas ut.|
| [fill_format](/cells/sv/python-net/aspose.cells.charts/floor/fill_format) | Representerar ett [Area.fill_format](/cells/sv/python-net/aspose.cells.drawing/area#fill_format)-objekt som innehåller fyllningsformateringsegenskaper för det angivna diagrammet eller formen.|
| [transparency](/cells/sv/python-net/aspose.cells.charts/floor/transparency) | Returnerar eller ställer in graden av transparens för området som ett värde från 0,0 (opak) till 1,0 (ren).|
| [border](/cells/sv/python-net/aspose.cells.charts/floor/border) | Hämtar eller sätter gränsen [Line](/cells/sv/python-net/aspose.cells.drawing/line).|



###  Exempel

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

###  Se även
* modul [aspose.cells.charts](..)
* klass [Area](/cells/sv/python-net/aspose.cells.drawing/area)
* klass [Floor](/cells/sv/python-net/aspose.cells.charts/floor)
* klass [Line](/cells/sv/python-net/aspose.cells.drawing/line)
