---
title: ChartDataTable classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 60
url: /fr/python-net/aspose.cells.charts/chartdatatable/
is_root: false
---
##  ChartDataTable classe
Représente une table de données de graphique.



Le type ChartDataTable expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [font](/cells/fr/python-net/aspose.cells.charts/chartdatatable/font) | Obtient un objet [ChartDataTable.font](/cells/fr/python-net/aspose.cells.charts/chartdatatable#font) qui représente le paramètre de police de la table de données de graphique spécifiée.|
| [auto_scale_font](/cells/fr/python-net/aspose.cells.charts/chartdatatable/auto_scale_font) | True si le texte de l'objet change de taille de police lorsque la taille de l'objet change.<br/> La valeur par défaut est Vrai.|
| [background_mode](/cells/fr/python-net/aspose.cells.charts/chartdatatable/background_mode) | Obtient et définit le mode d'affichage de l'arrière-plan|
| [background](/cells/fr/python-net/aspose.cells.charts/chartdatatable/background) | Obtient et définit le mode d'affichage de l'arrière-plan|
| [has_border_horizontal](/cells/fr/python-net/aspose.cells.charts/chartdatatable/has_border_horizontal) |True si la table de données du graphique a des bordures de cellule horizontales|
| [has_border_vertical](/cells/fr/python-net/aspose.cells.charts/chartdatatable/has_border_vertical) | True si la table de données du graphique comporte des bordures de cellule verticales|
| [has_border_outline](/cells/fr/python-net/aspose.cells.charts/chartdatatable/has_border_outline) | True si la table de données du graphique a des bordures de contour|
| [show_legend_key](/cells/fr/python-net/aspose.cells.charts/chartdatatable/show_legend_key) | True si la clé de légende de l'étiquette de données est visible.|
| [border](/cells/fr/python-net/aspose.cells.charts/chartdatatable/border) | Renvoie un objet Border qui représente la bordure de l'objet|



###  Exemples

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
chartIndex = worksheet.charts.add(ChartType.COLUMN, 5, 0, 25, 10)
# Accessing the instance of the newly added chart
chart = worksheet.charts[chartIndex]
# Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.n_series.add("A1:B3", True)
chart.show_data_table = True
# Getting Chart Table
chartTable = chart.chart_data_table
# Setting Chart Table Font Color
chartTable.font.color = Color.red
# Setting Legend Key VisibilityOptions
chartTable.show_legend_key = False
# Saving the Excel file
workbook.save("book1.xls")

```

###  Voir également
* module [aspose.cells.charts](..)
