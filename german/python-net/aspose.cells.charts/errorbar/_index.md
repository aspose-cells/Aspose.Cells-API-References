---
title: ErrorBar Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 150
url: /de/python-net/aspose.cells.charts/errorbar/
is_root: false
---
##  ErrorBar Klasse
Stellt den Fehlerbalken der Datenreihe dar.



**Nachlass:** [ErrorBar](/cells/python-net/aspose.cells.charts/errorbar) → 
[Line](/cells/de/python-net/aspose.cells.drawing/line)



Der Typ ErrorBar macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [compound_type](/cells/de/python-net/aspose.cells.charts/errorbar/compound_type) | Gibt den zusammengesetzten Linientyp an|
| [dash_type](/cells/de/python-net/aspose.cells.charts/errorbar/dash_type) | Gibt den Strichlinientyp an|
| [cap_type](/cells/de/python-net/aspose.cells.charts/errorbar/cap_type) | Gibt die Endkappen an.|
| [join_type](/cells/de/python-net/aspose.cells.charts/errorbar/join_type) | Gibt die Verbindungskappen an.|
| [begin_type](/cells/de/python-net/aspose.cells.charts/errorbar/begin_type) |Gibt eine Pfeilspitze für den Beginn einer Linie an.|
| [end_type](/cells/de/python-net/aspose.cells.charts/errorbar/end_type) | Gibt eine Pfeilspitze für das Ende einer Linie an.|
| [begin_arrow_length](/cells/de/python-net/aspose.cells.charts/errorbar/begin_arrow_length) | Gibt die Länge der Pfeilspitze für den Beginn einer Linie an.|
| [end_arrow_length](/cells/de/python-net/aspose.cells.charts/errorbar/end_arrow_length) | Gibt die Länge der Pfeilspitze für das Ende einer Linie an.|
| [begin_arrow_width](/cells/de/python-net/aspose.cells.charts/errorbar/begin_arrow_width) | Gibt die Breite der Pfeilspitze für den Beginn einer Linie an.|
| [end_arrow_width](/cells/de/python-net/aspose.cells.charts/errorbar/end_arrow_width) | Gibt die Breite der Pfeilspitze für das Ende einer Linie an.|
| [theme_color](/cells/de/python-net/aspose.cells.charts/errorbar/theme_color) | Ruft die Designfarbe ab und legt sie fest.|
| [color](/cells/de/python-net/aspose.cells.charts/errorbar/color) | Repräsentiert die Farbe der Linie.|
| [transparency](/cells/de/python-net/aspose.cells.charts/errorbar/transparency) | Gibt den Transparenzgrad der Linie als Wert von 0,0 (undurchsichtig) bis 1,0 (klar) zurück oder legt ihn fest.|
| [style](/cells/de/python-net/aspose.cells.charts/errorbar/style) | Repräsentiert den Stil der Linie.|
| [weight](/cells/de/python-net/aspose.cells.charts/errorbar/weight) | Ruft die [WeightType](/cells/de/python-net/aspose.cells.drawing/weighttype) der Leitung ab oder legt sie fest.|
| [weight_pt](/cells/de/python-net/aspose.cells.charts/errorbar/weight_pt) | Ruft die Gewichtung der Linie in Punkteinheiten ab oder legt diese fest.|
| [weight_px](/cells/de/python-net/aspose.cells.charts/errorbar/weight_px) | Ruft die Gewichtung der Linie in Pixeleinheiten ab oder legt diese fest.|
| [formatting_type](/cells/de/python-net/aspose.cells.charts/errorbar/formatting_type) | Ruft den Formattyp ab oder legt ihn fest.|
| [is_automatic_color](/cells/de/python-net/aspose.cells.charts/errorbar/is_automatic_color) | Gibt an, ob die Linienfarbe automatisch zugewiesen wird.|
| [is_visible](/cells/de/python-net/aspose.cells.charts/errorbar/is_visible) | Stellt dar, ob die Linie sichtbar ist.|
| [is_auto](/cells/de/python-net/aspose.cells.charts/errorbar/is_auto) | Gibt an, ob dieser Linienstil automatisch zugewiesen wird.|
| [gradient_fill](/cells/de/python-net/aspose.cells.charts/errorbar/gradient_fill) | Stellt eine Verlaufsfüllung dar.|
| [type](/cells/de/python-net/aspose.cells.charts/errorbar/type) |Repräsentiert den Betragstyp des Fehlerbalkens.|
| [display_type](/cells/de/python-net/aspose.cells.charts/errorbar/display_type) | Stellt den Anzeigetyp der Fehlerleiste dar.|
| [amount](/cells/de/python-net/aspose.cells.charts/errorbar/amount) | Repräsentiert die Menge des Fehlerbalkens.<br/> Der Betrag muss größer oder gleich Null sein.|
| [show_marker_t_top](/cells/de/python-net/aspose.cells.charts/errorbar/show_marker_t_top) | Gibt an, ob Fehlerbalken mit einem T-Top formatiert werden.|
| [plus_value](/cells/de/python-net/aspose.cells.charts/errorbar/plus_value) | Stellt den positiven Fehlerbetrag dar, wenn der Fehlerbalkentyp Benutzerdefiniert ist.|
| [minus_value](/cells/de/python-net/aspose.cells.charts/errorbar/minus_value) | Stellt den negativen Fehlerbetrag dar, wenn der Fehlerbalkentyp Benutzerdefiniert ist.|



###  Beispiele

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

###  Siehe auch
* Modul [aspose.cells.charts](..)
* Klasse [ErrorBar](/cells/de/python-net/aspose.cells.charts/errorbar)
* Klasse [Line](/cells/de/python-net/aspose.cells.drawing/line)
* Klasse [WeightType](/cells/de/python-net/aspose.cells.drawing/weighttype)
