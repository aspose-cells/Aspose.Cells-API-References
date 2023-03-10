---
title: Floor classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 160
url: /fr/python-net/aspose.cells.charts/floor/
is_root: false
---
##  Floor classe
Encapsule l'objet qui représente le plancher d'un graphique 3D.



**Héritage:** [Floor](/cells/python-net/aspose.cells.charts/floor) → 
[Area](/cells/fr/python-net/aspose.cells.drawing/area)



Le type Floor expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [background_color](/cells/fr/python-net/aspose.cells.charts/floor/background_color) | Obtient ou définit la couleur d'arrière-plan du [Area](/cells/fr/python-net/aspose.cells.drawing/area).|
| [foreground_color](/cells/fr/python-net/aspose.cells.charts/floor/foreground_color) | Obtient ou définit la couleur de premier plan.|
| [formatting](/cells/fr/python-net/aspose.cells.charts/floor/formatting) | Représente la mise en forme de la zone.|
| [invert_if_negative](/cells/fr/python-net/aspose.cells.charts/floor/invert_if_negative) | Si la propriété est vraie et que la valeur du point du graphique est un nombre négatif,<br/> la couleur de premier plan et la couleur d'arrière-plan seront échangées.|
| [fill_format](/cells/fr/python-net/aspose.cells.charts/floor/fill_format) | Représente un objet [Area.fill_format](/cells/fr/python-net/aspose.cells.drawing/area#fill_format) qui contient des propriétés de mise en forme de remplissage pour le graphique ou la forme spécifié.|
| [transparency](/cells/fr/python-net/aspose.cells.charts/floor/transparency) | Renvoie ou définit le degré de transparence de la zone sous la forme d'une valeur comprise entre 0,0 (opaque) et 1,0 (clair).|
| [border](/cells/fr/python-net/aspose.cells.charts/floor/border) | Obtient ou définit la bordure [Line](/cells/fr/python-net/aspose.cells.drawing/line).|



###  Exemple

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

###  Voir également
* module [aspose.cells.charts](..)
* classe [Area](/cells/fr/python-net/aspose.cells.drawing/area)
* classe [Floor](/cells/fr/python-net/aspose.cells.charts/floor)
* classe [Line](/cells/fr/python-net/aspose.cells.drawing/line)
