---
title: ChartArea Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 40
url: /de/python-net/aspose.cells.charts/chartarea/
is_root: false
---
##  ChartArea Klasse
Kapselt das Objekt, das den Diagrammbereich im Arbeitsblatt darstellt.



**Nachlass:** [ChartArea](/cells/python-net/aspose.cells.charts/chartarea) → 
[ChartFrame](/cells/de/python-net/aspose.cells.charts/chartframe)



Der Typ ChartArea macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [is_inner_mode](/cells/de/python-net/aspose.cells.charts/chartarea/is_inner_mode) | Gibt an, ob die Größe des Plotbereichs die Teilstriche und die Achsenbeschriftungen umfasst.<br/> False gibt an, dass die Größe die Größe des Plotbereichs, der Teilstriche und der Achsenbeschriftungen bestimmen soll.|
| [border](/cells/de/python-net/aspose.cells.charts/chartarea/border) | Ruft die [Line](/cells/de/python-net/aspose.cells.drawing/line) ab.|
| [area](/cells/de/python-net/aspose.cells.charts/chartarea/area) | Ruft die [ChartFrame.area](/cells/de/python-net/aspose.cells.charts/chartframe#area) ab.|
| [text_font](/cells/de/python-net/aspose.cells.charts/chartarea/text_font) | Ruft ein [ChartFrame.font](/cells/de/python-net/aspose.cells.charts/chartframe#font)-Objekt des angegebenen ChartFrame-Objekts ab.|
| [text_options](/cells/de/python-net/aspose.cells.charts/chartarea/text_options) | Ruft die Optionen des Textes ab und legt sie fest.|
| [font](/cells/de/python-net/aspose.cells.charts/chartarea/font) | Ruft ein [ChartArea.font](/cells/de/python-net/aspose.cells.charts/chartarea#font)-Objekt des angegebenen Chartarea-Objekts ab.|
| [auto_scale_font](/cells/de/python-net/aspose.cells.charts/chartarea/auto_scale_font) | True, wenn der Text im Objekt die Schriftgröße ändert, wenn sich die Objektgröße ändert. Der Standardwert ist True.|
| [background_mode](/cells/de/python-net/aspose.cells.charts/chartarea/background_mode) | Ruft den Anzeigemodus des Hintergrunds ab und legt ihn fest|
| [background](/cells/de/python-net/aspose.cells.charts/chartarea/background) | Ruft den Anzeigemodus des Hintergrunds ab und legt ihn fest|
| [is_automatic_size](/cells/de/python-net/aspose.cells.charts/chartarea/is_automatic_size) | Gibt an, ob die Größe des Diagrammrahmens automatisch angepasst wird.|
| [x](/cells/de/python-net/aspose.cells.charts/chartarea/x) | Ruft den horizontalen Versatz von der Spalte in der oberen linken Ecke ab oder ruft ihn ab.|
| [y](/cells/de/python-net/aspose.cells.charts/chartarea/y) |Ruft den vertikalen Versatz von der Zeile in der oberen linken Ecke ab oder ruft ihn ab.|
| [height](/cells/de/python-net/aspose.cells.charts/chartarea/height) | Ruft den vertikalen Versatz von der Zeile in der unteren rechten Ecke ab oder legt diesen fest.|
| [width](/cells/de/python-net/aspose.cells.charts/chartarea/width) | Ruft den horizontalen Versatz von der Spalte in der unteren rechten Ecke ab oder legt diesen fest.|
| [shadow](/cells/de/python-net/aspose.cells.charts/chartarea/shadow) | True, wenn der Rahmen einen Schatten hat.|
| [shape_properties](/cells/de/python-net/aspose.cells.charts/chartarea/shape_properties) | Ruft das [ChartFrame.shape_properties](/cells/de/python-net/aspose.cells.charts/chartframe#shape_properties)-Objekt ab.|
| [is_default_pos_be_set](/cells/de/python-net/aspose.cells.charts/chartarea/is_default_pos_be_set) | Gibt an, ob die Standardposition (DefaultX, DefaultY, DefaultWidth und DefaultHeight) festgelegt ist.|
| [default_x](/cells/de/python-net/aspose.cells.charts/chartarea/default_x) | Repräsentiert x der Standardposition|
| [default_y](/cells/de/python-net/aspose.cells.charts/chartarea/default_y) | Stellt y der Standardposition dar|
| [default_width](/cells/de/python-net/aspose.cells.charts/chartarea/default_width) | Repräsentiert die Breite der Standardposition|
| [default_height](/cells/de/python-net/aspose.cells.charts/chartarea/default_height) | Repräsentiert die Höhe der Standardposition|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [set_position_auto()](/cells/de/python-net/aspose.cells.charts/chartarea/set_position_auto/#) | Stellen Sie die Position des Rahmens auf automatisch|



###  Beispiel

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

###  Siehe auch
* Modul [aspose.cells.charts](..)
* Klasse [ChartArea](/cells/de/python-net/aspose.cells.charts/chartarea)
* Klasse [ChartFrame](/cells/de/python-net/aspose.cells.charts/chartframe)
* Klasse [Line](/cells/de/python-net/aspose.cells.drawing/line)
