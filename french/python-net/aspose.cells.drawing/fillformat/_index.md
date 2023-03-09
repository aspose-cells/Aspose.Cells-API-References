---
title: FillFormat classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 180
url: /fr/python-net/aspose.cells.drawing/fillformat/
is_root: false
---
##  FillFormat classe
Encapsule l'objet qui représente la mise en forme de remplissage d'une forme.



Le type FillFormat expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [type](/cells/fr/python-net/aspose.cells.drawing/fillformat/type) |Obtient et définit le type de remplissage.|
| [fill_type](/cells/fr/python-net/aspose.cells.drawing/fillformat/fill_type) | Obtient et définit le type de remplissage|
| [transparency](/cells/fr/python-net/aspose.cells.drawing/fillformat/transparency) | Renvoie ou définit le degré de transparence de la zone sous la forme d'une valeur comprise entre 0,0 (opaque) et 1,0 (clair).|
| [set_type](/cells/fr/python-net/aspose.cells.drawing/fillformat/set_type) | Obtient le type de jeu de format de remplissage.|
| [gradient_fill](/cells/fr/python-net/aspose.cells.drawing/fillformat/gradient_fill) | Obtient l'objet [FillFormat.gradient_fill](/cells/fr/python-net/aspose.cells.drawing/fillformat#gradient_fill).|
| [texture_fill](/cells/fr/python-net/aspose.cells.drawing/fillformat/texture_fill) | Obtient l'objet [FillFormat.texture_fill](/cells/fr/python-net/aspose.cells.drawing/fillformat#texture_fill).|
| [solid_fill](/cells/fr/python-net/aspose.cells.drawing/fillformat/solid_fill) | Obtient l'objet [FillFormat.solid_fill](/cells/fr/python-net/aspose.cells.drawing/fillformat#solid_fill).|
| [pattern_fill](/cells/fr/python-net/aspose.cells.drawing/fillformat/pattern_fill) | Obtient l'objet [FillFormat.pattern_fill](/cells/fr/python-net/aspose.cells.drawing/fillformat#pattern_fill).|
| [gradient_color_type](/cells/fr/python-net/aspose.cells.drawing/fillformat/gradient_color_type) | Renvoie le type de couleur de dégradé pour le remplissage spécifié.|
| [gradient_style](/cells/fr/python-net/aspose.cells.drawing/fillformat/gradient_style) | Renvoie le style de dégradé pour le remplissage spécifié.|
| [gradient_color1](/cells/fr/python-net/aspose.cells.drawing/fillformat/gradient_color1) | Renvoie la couleur de dégradé 1 pour le remplissage spécifié.|
| [gradient_color2](/cells/fr/python-net/aspose.cells.drawing/fillformat/gradient_color2) | Renvoie la couleur de dégradé 2 pour le remplissage spécifié.|
| [gradient_degree](/cells/fr/python-net/aspose.cells.drawing/fillformat/gradient_degree) | Renvoie le degré de dégradé pour le remplissage spécifié.<br/> Ne s'applique qu'à Excel 2007.|
| [gradient_variant](/cells/fr/python-net/aspose.cells.drawing/fillformat/gradient_variant) | Renvoie la variante de dégradé pour le remplissage spécifié.<br/> Ne s'applique qu'à Excel 2007.|
| [preset_color](/cells/fr/python-net/aspose.cells.drawing/fillformat/preset_color) | Renvoie la couleur prédéfinie du dégradé pour le remplissage spécifié.|
| [texture](/cells/fr/python-net/aspose.cells.drawing/fillformat/texture) | Représente le type de texture pour le remplissage spécifié.|
| [pattern](/cells/fr/python-net/aspose.cells.drawing/fillformat/pattern) | Représente le modèle d'affichage d'une zone.|
| [picture_format_type](/cells/fr/python-net/aspose.cells.drawing/fillformat/picture_format_type) | Obtient et définit le type de format d'image.|
| [scale](/cells/fr/python-net/aspose.cells.drawing/fillformat/scale) | Obtient et définit l'échelle du format d'image.|
| [image_data](/cells/fr/python-net/aspose.cells.drawing/fillformat/image_data) | Obtient et définit les données d'image de l'image.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [set_two_color_gradient(color1, color2, style, variant)](/cells/fr/python-net/aspose.cells.drawing/fillformat/set_two_color_gradient/#aspose.pydrawing.Color-aspose.pydrawing.Color-GradientStyleType-int) | Définit le remplissage spécifié sur un dégradé bicolore.<br/> Ne s'applique qu'à Excel 2007.|
| [set_two_color_gradient(color1, transparency1, color2, transparency2, style, variant)](/cells/fr/python-net/aspose.cells.drawing/fillformat/set_two_color_gradient/#aspose.pydrawing.Color-float-aspose.pydrawing.Color-float-GradientStyleType-int) | Définit le remplissage spécifié sur un dégradé bicolore.<br/> Ne s'applique qu'à Excel 2007.|
| [set_one_color_gradient(color, degree, style, variant)](/cells/fr/python-net/aspose.cells.drawing/fillformat/set_one_color_gradient/#aspose.pydrawing.Color-float-GradientStyleType-int) | Définit le remplissage spécifié sur un dégradé d'une seule couleur.<br/> Ne s'applique qu'à Excel 2007.|
| [set_preset_color_gradient(preset_color, style, variant)](/cells/fr/python-net/aspose.cells.drawing/fillformat/set_preset_color_gradient/#GradientPresetType-GradientStyleType-int) | Définit le remplissage spécifié sur un dégradé de couleur prédéfini.<br/> Ne s'applique qu'à Excel 2007.|



###  Exemples

```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartType
from aspose.cells.drawing import GradientStyleType
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
# Adding a new worksheet to the Excel object
sheetIndex = workbook.worksheets.add()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[sheetIndex]
# Adding a sample value to "A1" cell
worksheet.cells.get("A1").put_value(50)
# Adding a sample value to "A2" cell
worksheet.cells.get("A2").put_value(100)
# Adding a sample value to "A3" cell
worksheet.cells.get("A3").put_value(150)
# Adding a sample value to "A4" cell
worksheet.cells.get("A4").put_value(200)
# Adding a sample value to "B1" cell
worksheet.cells.get("B1").put_value(60)
# Adding a sample value to "B2" cell
worksheet.cells.get("B2").put_value(32)
# Adding a sample value to "B3" cell
worksheet.cells.get("B3").put_value(50)
# Adding a sample value to "B4" cell
worksheet.cells.get("B4").put_value(40)
# Adding a sample value to "C1" cell as category data
worksheet.cells.get("C1").put_value("Q1")
# Adding a sample value to "C2" cell as category data
worksheet.cells.get("C2").put_value("Q2")
# Adding a sample value to "C3" cell as category data
worksheet.cells.get("C3").put_value("Y1")
# Adding a sample value to "C4" cell as category data
worksheet.cells.get("C4").put_value("Y2")
# Adding a chart to the worksheet
chartIndex = worksheet.charts.add(ChartType.COLUMN, 5, 0, 15, 5)
# Accessing the instance of the newly added chart
chart = worksheet.charts[chartIndex]
# Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
seriesIndex = chart.n_series.add("A1:B4", True)
# Setting the data source for the category data of NSeries
chart.n_series.category_data = "C1:C4"
# Filling the area of the 2nd NSeries with a gradient
chart.n_series[seriesIndex].area.fill_format.set_one_color_gradient(Color.lime, 1, GradientStyleType.HORIZONTAL, 1)

```

###  Voir également
* module [aspose.cells.drawing](..)
