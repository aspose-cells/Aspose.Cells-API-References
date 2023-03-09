---
title: classe Floor
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 160
url: /it/python-net/aspose.cells.charts/floor/
is_root: false
---
##  classe Floor
Incapsula l'oggetto che rappresenta la base di un grafico 3D.



**Eredità:** [Floor](/cells/python-net/aspose.cells.charts/floor) → 
[Area](/cells/it/python-net/aspose.cells.drawing/area)



Il tipo Floor espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [background_color](/cells/it/python-net/aspose.cells.charts/floor/background_color) | Ottiene o imposta il colore di sfondo di [Area](/cells/it/python-net/aspose.cells.drawing/area).|
| [foreground_color](/cells/it/python-net/aspose.cells.charts/floor/foreground_color) | Ottiene o imposta il Color in primo piano.|
| [formatting](/cells/it/python-net/aspose.cells.charts/floor/formatting) | Rappresenta la formattazione dell'area.|
| [invert_if_negative](/cells/it/python-net/aspose.cells.charts/floor/invert_if_negative) | Se la proprietà è vera e il valore del punto del grafico è un numero negativo,<br/> il colore di primo piano e il colore di sfondo verranno scambiati.|
| [fill_format](/cells/it/python-net/aspose.cells.charts/floor/fill_format) | Rappresenta un oggetto [Area.fill_format](/cells/it/python-net/aspose.cells.drawing/area#fill_format) che contiene le proprietà di formattazione del riempimento per il grafico o la forma specificati.|
| [transparency](/cells/it/python-net/aspose.cells.charts/floor/transparency) | Restituisce o imposta il grado di trasparenza dell'area come valore compreso tra 0,0 (opaco) e 1,0 (trasparente).|
| [border](/cells/it/python-net/aspose.cells.charts/floor/border) | Ottiene o imposta il bordo [Line](/cells/it/python-net/aspose.cells.drawing/line).|



###  Esempi

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

###  Guarda anche
* modulo [aspose.cells.charts](..)
* classe [Area](/cells/it/python-net/aspose.cells.drawing/area)
* classe [Floor](/cells/it/python-net/aspose.cells.charts/floor)
* classe [Line](/cells/it/python-net/aspose.cells.drawing/line)
