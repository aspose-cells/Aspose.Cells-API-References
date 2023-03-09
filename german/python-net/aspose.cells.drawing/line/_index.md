---
title: Line Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 290
url: /de/python-net/aspose.cells.drawing/line/
is_root: false
---
##  Line Klasse
Kapselt das Objekt, das das Linienformat darstellt.



Der Typ Line macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [compound_type](/cells/de/python-net/aspose.cells.drawing/line/compound_type) | Gibt den zusammengesetzten Linientyp an|
| [dash_type](/cells/de/python-net/aspose.cells.drawing/line/dash_type) | Gibt den Strichlinientyp an|
| [cap_type](/cells/de/python-net/aspose.cells.drawing/line/cap_type) | Gibt die Endkappen an.|
| [join_type](/cells/de/python-net/aspose.cells.drawing/line/join_type) | Gibt die Verbindungskappen an.|
| [begin_type](/cells/de/python-net/aspose.cells.drawing/line/begin_type) |Gibt eine Pfeilspitze für den Beginn einer Linie an.|
| [end_type](/cells/de/python-net/aspose.cells.drawing/line/end_type) | Gibt eine Pfeilspitze für das Ende einer Linie an.|
| [begin_arrow_length](/cells/de/python-net/aspose.cells.drawing/line/begin_arrow_length) | Gibt die Länge der Pfeilspitze für den Beginn einer Linie an.|
| [end_arrow_length](/cells/de/python-net/aspose.cells.drawing/line/end_arrow_length) | Gibt die Länge der Pfeilspitze für das Ende einer Linie an.|
| [begin_arrow_width](/cells/de/python-net/aspose.cells.drawing/line/begin_arrow_width) | Gibt die Breite der Pfeilspitze für den Beginn einer Linie an.|
| [end_arrow_width](/cells/de/python-net/aspose.cells.drawing/line/end_arrow_width) | Gibt die Breite der Pfeilspitze für das Ende einer Linie an.|
| [theme_color](/cells/de/python-net/aspose.cells.drawing/line/theme_color) | Ruft die Designfarbe ab und legt sie fest.|
| [color](/cells/de/python-net/aspose.cells.drawing/line/color) | Repräsentiert die Farbe der Linie.|
| [transparency](/cells/de/python-net/aspose.cells.drawing/line/transparency) | Gibt den Transparenzgrad der Linie als Wert von 0,0 (undurchsichtig) bis 1,0 (klar) zurück oder legt ihn fest.|
| [style](/cells/de/python-net/aspose.cells.drawing/line/style) | Repräsentiert den Stil der Linie.|
| [weight](/cells/de/python-net/aspose.cells.drawing/line/weight) | Ruft die [WeightType](/cells/de/python-net/aspose.cells.drawing/weighttype) der Leitung ab oder legt sie fest.|
| [weight_pt](/cells/de/python-net/aspose.cells.drawing/line/weight_pt) | Ruft die Gewichtung der Linie in Punkteinheiten ab oder legt diese fest.|
| [weight_px](/cells/de/python-net/aspose.cells.drawing/line/weight_px) | Ruft die Gewichtung der Linie in Pixeleinheiten ab oder legt diese fest.|
| [formatting_type](/cells/de/python-net/aspose.cells.drawing/line/formatting_type) | Ruft den Formattyp ab oder legt ihn fest.|
| [is_automatic_color](/cells/de/python-net/aspose.cells.drawing/line/is_automatic_color) | Gibt an, ob die Linienfarbe automatisch zugewiesen wird.|
| [is_visible](/cells/de/python-net/aspose.cells.drawing/line/is_visible) | Stellt dar, ob die Linie sichtbar ist.|
| [is_auto](/cells/de/python-net/aspose.cells.drawing/line/is_auto) | Gibt an, ob dieser Linienstil automatisch zugewiesen wird.|
| [gradient_fill](/cells/de/python-net/aspose.cells.drawing/line/gradient_fill) | Stellt eine Verlaufsfüllung dar.|



###  Beispiele

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

###  Siehe auch
* Modul [aspose.cells.drawing](..)
* Klasse [WeightType](/cells/de/python-net/aspose.cells.drawing/weighttype)
