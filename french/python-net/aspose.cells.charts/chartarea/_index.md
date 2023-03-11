---
title: ChartArea classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 40
url: /fr/python-net/aspose.cells.charts/chartarea/
is_root: false
---
##  ChartArea classe
Encapsule l'objet qui représente la zone de graphique dans la feuille de calcul.



**Héritage:** [ChartArea](/cells/python-net/aspose.cells.charts/chartarea) → 
[ChartFrame](/cells/fr/python-net/aspose.cells.charts/chartframe)



Le type ChartArea expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [is_inner_mode](/cells/fr/python-net/aspose.cells.charts/chartarea/is_inner_mode) | Indique si la taille de la zone de tracé inclut les graduations et les étiquettes des axes.<br/> False spécifie que la taille doit déterminer la taille de la zone de tracé, les graduations et les étiquettes des axes.|
| [border](/cells/fr/python-net/aspose.cells.charts/chartarea/border) | Obtient le [Line](/cells/fr/python-net/aspose.cells.drawing/line).|
| [area](/cells/fr/python-net/aspose.cells.charts/chartarea/area) | Obtient le [ChartFrame.area](/cells/fr/python-net/aspose.cells.charts/chartframe#area).|
| [text_font](/cells/fr/python-net/aspose.cells.charts/chartarea/text_font) | Obtient un objet [ChartFrame.font](/cells/fr/python-net/aspose.cells.charts/chartframe#font) de l'objet ChartFrame spécifié.|
| [text_options](/cells/fr/python-net/aspose.cells.charts/chartarea/text_options) | Obtient et définit les options du texte.|
| [font](/cells/fr/python-net/aspose.cells.charts/chartarea/font) | Obtient un objet [ChartArea.font](/cells/fr/python-net/aspose.cells.charts/chartarea#font) de l'objet chartarea spécifié.|
| [auto_scale_font](/cells/fr/python-net/aspose.cells.charts/chartarea/auto_scale_font) | True si le texte de l'objet change de taille de police lorsque la taille de l'objet change. La valeur par défaut est Vrai.|
| [background_mode](/cells/fr/python-net/aspose.cells.charts/chartarea/background_mode) | Obtient et définit le mode d'affichage de l'arrière-plan|
| [background](/cells/fr/python-net/aspose.cells.charts/chartarea/background) | Obtient et définit le mode d'affichage de l'arrière-plan|
| [is_automatic_size](/cells/fr/python-net/aspose.cells.charts/chartarea/is_automatic_size) | Indique si le cadre du graphique est dimensionné automatiquement.|
| [x](/cells/fr/python-net/aspose.cells.charts/chartarea/x) | Obtient ou obtient le décalage horizontal à partir de sa colonne d'angle supérieur gauche.|
| [y](/cells/fr/python-net/aspose.cells.charts/chartarea/y) |Obtient ou obtient le décalage vertical à partir de sa ligne de coin supérieur gauche.|
| [height](/cells/fr/python-net/aspose.cells.charts/chartarea/height) | Obtient ou définit le décalage vertical à partir de sa ligne du coin inférieur droit.|
| [width](/cells/fr/python-net/aspose.cells.charts/chartarea/width) | Obtient ou définit le décalage horizontal à partir de sa colonne d'angle inférieur droit.|
| [shadow](/cells/fr/python-net/aspose.cells.charts/chartarea/shadow) | Vrai si le cadre a une ombre.|
| [shape_properties](/cells/fr/python-net/aspose.cells.charts/chartarea/shape_properties) | Obtient l'objet [ChartFrame.shape_properties](/cells/fr/python-net/aspose.cells.charts/chartframe#shape_properties).|
| [is_default_pos_be_set](/cells/fr/python-net/aspose.cells.charts/chartarea/is_default_pos_be_set) | Indique si la position par défaut (DefaultX, DefaultY, DefaultWidth et DefaultHeight) est définie.|
| [default_x](/cells/fr/python-net/aspose.cells.charts/chartarea/default_x) | Représente x de la position par défaut|
| [default_y](/cells/fr/python-net/aspose.cells.charts/chartarea/default_y) | Représente y de la position par défaut|
| [default_width](/cells/fr/python-net/aspose.cells.charts/chartarea/default_width) | Représente la largeur de la position par défaut|
| [default_height](/cells/fr/python-net/aspose.cells.charts/chartarea/default_height) | Représente la hauteur de la position par défaut|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [set_position_auto()](/cells/fr/python-net/aspose.cells.charts/chartarea/set_position_auto/#) | Régler la position du cadre sur automatique|



###  Exemple

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
chartIndex = worksheet.charts.add(ChartType.COLUMN, 5, 0, 15, 5)
# Accessing the instance of the newly added chart
chart = worksheet.charts[chartIndex]
# Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.n_series.add("A1:B3", True)
# Getting Chart Area
chartArea = chart.chart_area
# Setting the foreground color of the chart area
chartArea.area.foreground_color = Color.yellow
# Setting Chart Area Shadow
chartArea.shadow = True
# Saving the Excel file
workbook.save("book1.xls")

```

###  Voir également
* module [aspose.cells.charts](..)
* classe [ChartArea](/cells/fr/python-net/aspose.cells.charts/chartarea)
* classe [ChartFrame](/cells/fr/python-net/aspose.cells.charts/chartframe)
* classe [Line](/cells/fr/python-net/aspose.cells.drawing/line)
