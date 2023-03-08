---
title: Floor Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 160
url: /de/python-net/aspose.cells.charts/floor/
is_root: false
---
##  Floor Klasse
Kapselt das Objekt, das den Boden eines 3D-Diagramms darstellt.



**Nachlass:** [Floor](/cells/python-net/aspose.cells.charts/floor) → 
[Area](/cells/de/python-net/aspose.cells.drawing/area)



Der Typ Floor macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [background_color](/cells/de/python-net/aspose.cells.charts/floor/background_color) | Ruft die Hintergrundfarbe von [Area](/cells/de/python-net/aspose.cells.drawing/area) ab oder legt sie fest.|
| [foreground_color](/cells/de/python-net/aspose.cells.charts/floor/foreground_color) | Ruft die Vordergrundfarbe ab oder legt sie fest.|
| [formatting](/cells/de/python-net/aspose.cells.charts/floor/formatting) | Repräsentiert die Formatierung des Bereichs.|
| [invert_if_negative](/cells/de/python-net/aspose.cells.charts/floor/invert_if_negative) | Wenn die Eigenschaft wahr ist und der Wert des Diagrammpunkts eine negative Zahl ist,<br/> Vorder- und Hintergrundfarbe werden vertauscht.|
| [fill_format](/cells/de/python-net/aspose.cells.charts/floor/fill_format) | Stellt ein [Area.fill_format](/cells/de/python-net/aspose.cells.drawing/area#fill_format)-Objekt dar, das Füllformatierungseigenschaften für das angegebene Diagramm oder Shape enthält.|
| [transparency](/cells/de/python-net/aspose.cells.charts/floor/transparency) | Gibt den Transparenzgrad des Bereichs als Wert von 0,0 (deckend) bis 1,0 (durchsichtig) zurück oder legt ihn fest.|
| [border](/cells/de/python-net/aspose.cells.charts/floor/border) | Ruft die Grenze [Line](/cells/de/python-net/aspose.cells.drawing/line) ab oder legt sie fest.|



###  Beispiel

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

###  Siehe auch
* Modul [aspose.cells.charts](..)
* Klasse [Area](/cells/de/python-net/aspose.cells.drawing/area)
* Klasse [Floor](/cells/de/python-net/aspose.cells.charts/floor)
* Klasse [Line](/cells/de/python-net/aspose.cells.drawing/line)
