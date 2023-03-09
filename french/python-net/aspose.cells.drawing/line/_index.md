---
title: Line classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 290
url: /fr/python-net/aspose.cells.drawing/line/
is_root: false
---
##  Line classe
Encapsule l'objet qui représente le format de ligne.



Le type Line expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [compound_type](/cells/fr/python-net/aspose.cells.drawing/line/compound_type) |Spécifie le type de ligne composée|
| [dash_type](/cells/fr/python-net/aspose.cells.drawing/line/dash_type) | Spécifie le type de ligne pointillée|
| [cap_type](/cells/fr/python-net/aspose.cells.drawing/line/cap_type) | Spécifie les majuscules de fin.|
| [join_type](/cells/fr/python-net/aspose.cells.drawing/line/join_type) | Spécifie les bouchons de jointure.|
| [begin_type](/cells/fr/python-net/aspose.cells.drawing/line/begin_type) | Spécifie une pointe de flèche pour le début d'une ligne.|
| [end_type](/cells/fr/python-net/aspose.cells.drawing/line/end_type) | Spécifie une pointe de flèche pour la fin d'une ligne.|
| [begin_arrow_length](/cells/fr/python-net/aspose.cells.drawing/line/begin_arrow_length) | Spécifie la longueur de la pointe de flèche pour le début d'une ligne.|
| [end_arrow_length](/cells/fr/python-net/aspose.cells.drawing/line/end_arrow_length) | Spécifie la longueur de la pointe de flèche pour la fin d'une ligne.|
| [begin_arrow_width](/cells/fr/python-net/aspose.cells.drawing/line/begin_arrow_width) | Spécifie la largeur de la pointe de flèche pour le début d'une ligne.|
| [end_arrow_width](/cells/fr/python-net/aspose.cells.drawing/line/end_arrow_width) | Spécifie la largeur de la pointe de flèche pour la fin d'une ligne.|
| [theme_color](/cells/fr/python-net/aspose.cells.drawing/line/theme_color) | Obtient et définit la couleur du thème.|
| [color](/cells/fr/python-net/aspose.cells.drawing/line/color) | Représente la Couleur de la ligne.|
| [transparency](/cells/fr/python-net/aspose.cells.drawing/line/transparency) | Renvoie ou définit le degré de transparence de la ligne sous la forme d'une valeur comprise entre 0,0 (opaque) et 1,0 (clair).|
| [style](/cells/fr/python-net/aspose.cells.drawing/line/style) | Représente le style de la ligne.|
| [weight](/cells/fr/python-net/aspose.cells.drawing/line/weight) | Obtient ou définit le [WeightType](/cells/fr/python-net/aspose.cells.drawing/weighttype) de la ligne.|
| [weight_pt](/cells/fr/python-net/aspose.cells.drawing/line/weight_pt) | Obtient ou définit l'épaisseur de la ligne en unités de points.|
| [weight_px](/cells/fr/python-net/aspose.cells.drawing/line/weight_px) | Obtient ou définit l'épaisseur de la ligne en pixels.|
| [formatting_type](/cells/fr/python-net/aspose.cells.drawing/line/formatting_type) | Obtient ou définit le type de format.|
| [is_automatic_color](/cells/fr/python-net/aspose.cells.drawing/line/is_automatic_color) |Indique si la couleur de la ligne est attribuée automatiquement.|
| [is_visible](/cells/fr/python-net/aspose.cells.drawing/line/is_visible) | Indique si la ligne est visible.|
| [is_auto](/cells/fr/python-net/aspose.cells.drawing/line/is_auto) | Indique si ce style de ligne est attribué automatiquement.|
| [gradient_fill](/cells/fr/python-net/aspose.cells.drawing/line/gradient_fill) | Représente le remplissage dégradé.|



###  Exemple

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

###  Voir également
* module [aspose.cells.drawing](..)
* classe [WeightType](/cells/fr/python-net/aspose.cells.drawing/weighttype)
