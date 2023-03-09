---
title: ErrorBar classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 150
url: /fr/python-net/aspose.cells.charts/errorbar/
is_root: false
---
##  ErrorBar classe
Représente la barre d'erreur de la série de données.



**Héritage:** [ErrorBar](/cells/python-net/aspose.cells.charts/errorbar) → 
[Line](/cells/fr/python-net/aspose.cells.drawing/line)



Le type ErrorBar expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [compound_type](/cells/fr/python-net/aspose.cells.charts/errorbar/compound_type) |Spécifie le type de ligne composée|
| [dash_type](/cells/fr/python-net/aspose.cells.charts/errorbar/dash_type) | Spécifie le type de ligne pointillée|
| [cap_type](/cells/fr/python-net/aspose.cells.charts/errorbar/cap_type) | Spécifie les majuscules de fin.|
| [join_type](/cells/fr/python-net/aspose.cells.charts/errorbar/join_type) | Spécifie les bouchons de jointure.|
| [begin_type](/cells/fr/python-net/aspose.cells.charts/errorbar/begin_type) | Spécifie une pointe de flèche pour le début d'une ligne.|
| [end_type](/cells/fr/python-net/aspose.cells.charts/errorbar/end_type) | Spécifie une pointe de flèche pour la fin d'une ligne.|
| [begin_arrow_length](/cells/fr/python-net/aspose.cells.charts/errorbar/begin_arrow_length) | Spécifie la longueur de la pointe de flèche pour le début d'une ligne.|
| [end_arrow_length](/cells/fr/python-net/aspose.cells.charts/errorbar/end_arrow_length) | Spécifie la longueur de la pointe de flèche pour la fin d'une ligne.|
| [begin_arrow_width](/cells/fr/python-net/aspose.cells.charts/errorbar/begin_arrow_width) | Spécifie la largeur de la pointe de flèche pour le début d'une ligne.|
| [end_arrow_width](/cells/fr/python-net/aspose.cells.charts/errorbar/end_arrow_width) | Spécifie la largeur de la pointe de flèche pour la fin d'une ligne.|
| [theme_color](/cells/fr/python-net/aspose.cells.charts/errorbar/theme_color) | Obtient et définit la couleur du thème.|
| [color](/cells/fr/python-net/aspose.cells.charts/errorbar/color) | Représente la Couleur de la ligne.|
| [transparency](/cells/fr/python-net/aspose.cells.charts/errorbar/transparency) | Renvoie ou définit le degré de transparence de la ligne sous la forme d'une valeur comprise entre 0,0 (opaque) et 1,0 (clair).|
| [style](/cells/fr/python-net/aspose.cells.charts/errorbar/style) | Représente le style de la ligne.|
| [weight](/cells/fr/python-net/aspose.cells.charts/errorbar/weight) | Obtient ou définit le [WeightType](/cells/fr/python-net/aspose.cells.drawing/weighttype) de la ligne.|
| [weight_pt](/cells/fr/python-net/aspose.cells.charts/errorbar/weight_pt) | Obtient ou définit l'épaisseur de la ligne en unités de points.|
| [weight_px](/cells/fr/python-net/aspose.cells.charts/errorbar/weight_px) | Obtient ou définit l'épaisseur de la ligne en pixels.|
| [formatting_type](/cells/fr/python-net/aspose.cells.charts/errorbar/formatting_type) | Obtient ou définit le type de format.|
| [is_automatic_color](/cells/fr/python-net/aspose.cells.charts/errorbar/is_automatic_color) |Indique si la couleur de la ligne est attribuée automatiquement.|
| [is_visible](/cells/fr/python-net/aspose.cells.charts/errorbar/is_visible) | Indique si la ligne est visible.|
| [is_auto](/cells/fr/python-net/aspose.cells.charts/errorbar/is_auto) | Indique si ce style de ligne est attribué automatiquement.|
| [gradient_fill](/cells/fr/python-net/aspose.cells.charts/errorbar/gradient_fill) | Représente le remplissage dégradé.|
| [type](/cells/fr/python-net/aspose.cells.charts/errorbar/type) | Représente le type de montant de la barre d'erreur.|
| [display_type](/cells/fr/python-net/aspose.cells.charts/errorbar/display_type) | Représente le type d'affichage de la barre d'erreur.|
| [amount](/cells/fr/python-net/aspose.cells.charts/errorbar/amount) | Représente la quantité de barre d'erreur.<br/> Le montant doit être supérieur ou égal à zéro.|
| [show_marker_t_top](/cells/fr/python-net/aspose.cells.charts/errorbar/show_marker_t_top) | Indique si le formatage des barres d'erreur avec un T-top.|
| [plus_value](/cells/fr/python-net/aspose.cells.charts/errorbar/plus_value) | Représente un montant d'erreur positif lorsque le type de barre d'erreur est Personnalisé.|
| [minus_value](/cells/fr/python-net/aspose.cells.charts/errorbar/minus_value) | Représente le montant d'erreur négatif lorsque le type de barre d'erreur est Personnalisé.|



###  Exemple

```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartType, ErrorBarDisplayType, ErrorBarType

workbook = Workbook()
cells = workbook.worksheets[0].cells
cells.get("a1").put_value(2)
cells.get("a2").put_value(5)
cells.get("a3").put_value(3)
cells.get("a4").put_value(6)
cells.get("b1").put_value(4)
cells.get("b2").put_value(3)
cells.get("b3").put_value(6)
cells.get("b4").put_value(7)
cells.get("C1").put_value("Q1")
cells.get("C2").put_value("Q2")
cells.get("C3").put_value("Y1")
cells.get("C4").put_value("Y2")
chartIndex = workbook.worksheets[0].charts.add(ChartType.COLUMN, 11, 0, 27, 10)
chart = workbook.worksheets[0].charts[chartIndex]
chart.n_series.add("A1:B4", True)
chart.n_series.category_data = "C1:C4"
for i in range(len(chart.NSeries)):
    aseries = chart.n_series[i]
    aseries.y_error_bar.display_type = ErrorBarDisplayType.MINUS
    aseries.y_error_bar.type = ErrorBarType.FIXED_VALUE
    aseries.y_error_bar.amount = 5

```

###  Voir également
* module [aspose.cells.charts](..)
* classe [ErrorBar](/cells/fr/python-net/aspose.cells.charts/errorbar)
* classe [Line](/cells/fr/python-net/aspose.cells.drawing/line)
* classe [WeightType](/cells/fr/python-net/aspose.cells.drawing/weighttype)
