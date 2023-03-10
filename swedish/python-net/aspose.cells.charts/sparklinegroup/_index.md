---
title: SparklineGroup klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 280
url: /sv/python-net/aspose.cells.charts/sparklinegroup/
is_root: false
---
##  SparklineGroup klass
[Sparkline](/cells/sv/python-net/aspose.cells.charts/sparkline) är organiserad i sparkline-grupp. En SparklineGroup innehåller ett varierande antal sparkline-objekt.
En sparkline-grupp anger typ, visningsinställningar och axelinställningar för sparklines.



Typen SparklineGroup avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [preset_style](/cells/sv/python-net/aspose.cells.charts/sparklinegroup/preset_style) | Hämtar och ställer in den förinställda stiltypen för sparklinegruppen.|
| [sparkline_collection](/cells/sv/python-net/aspose.cells.charts/sparklinegroup/sparkline_collection) | Får samlingen av [Sparkline](/cells/sv/python-net/aspose.cells.charts/sparkline) objekt.|
| [sparklines](/cells/sv/python-net/aspose.cells.charts/sparklinegroup/sparklines) | Får samlingen av [Sparkline](/cells/sv/python-net/aspose.cells.charts/sparkline) objekt.|
| [type](/cells/sv/python-net/aspose.cells.charts/sparklinegroup/type) | Indikerar sparkline-typen för sparklinegruppen.|
| [plot_empty_cells_type](/cells/sv/python-net/aspose.cells.charts/sparklinegroup/plot_empty_cells_type) | Indikerar hur tomma celler plottas.|
| [display_hidden](/cells/sv/python-net/aspose.cells.charts/sparklinegroup/display_hidden) |Anger om data ska visas i dolda rader och kolumner.|
| [show_high_point](/cells/sv/python-net/aspose.cells.charts/sparklinegroup/show_high_point) | Indikerar om de högsta punkterna med data i sparklinegruppen ska markeras.|
| [high_point_color](/cells/sv/python-net/aspose.cells.charts/sparklinegroup/high_point_color) | Hämtar och ställer in färgen på de högsta datapunkterna i sparklinegruppen.|
| [show_low_point](/cells/sv/python-net/aspose.cells.charts/sparklinegroup/show_low_point) | Indikerar om de lägsta datapunkterna i sparklinegruppen ska markeras.|
| [low_point_color](/cells/sv/python-net/aspose.cells.charts/sparklinegroup/low_point_color) | Hämtar och ställer in färgen på de lägsta datapunkterna i sparklinegruppen.|
| [show_negative_points](/cells/sv/python-net/aspose.cells.charts/sparklinegroup/show_negative_points) | Indikerar om de negativa värdena på sparklinegruppen ska markeras med en annan färg eller markör.|
| [negative_points_color](/cells/sv/python-net/aspose.cells.charts/sparklinegroup/negative_points_color) | Hämtar och ställer in färgen på de negativa värdena på sparklinegruppen.|
| [show_first_point](/cells/sv/python-net/aspose.cells.charts/sparklinegroup/show_first_point) | Indikerar om den första datapunkten i sparklinegruppen ska markeras.|
| [first_point_color](/cells/sv/python-net/aspose.cells.charts/sparklinegroup/first_point_color) | Hämtar och ställer in färgen på den första datapunkten i sparklinegruppen.|
| [show_last_point](/cells/sv/python-net/aspose.cells.charts/sparklinegroup/show_last_point) | Indikerar om den sista datapunkten i sparklinegruppen ska markeras.|
| [last_point_color](/cells/sv/python-net/aspose.cells.charts/sparklinegroup/last_point_color) | Hämtar och ställer in färgen på den sista datapunkten i sparklinegruppen.|
| [show_markers](/cells/sv/python-net/aspose.cells.charts/sparklinegroup/show_markers) |Indikerar om varje punkt i varje linje sparkline i sparklinegruppen ska markeras.|
| [markers_color](/cells/sv/python-net/aspose.cells.charts/sparklinegroup/markers_color) | Hämtar och ställer in färgen på punkterna i varje linje sparkline i sparklinegruppen.|
| [series_color](/cells/sv/python-net/aspose.cells.charts/sparklinegroup/series_color) | Får och ställer in färgen på sparklines i sparklinegruppen.|
| [plot_right_to_left](/cells/sv/python-net/aspose.cells.charts/sparklinegroup/plot_right_to_left) | Indikerar om plotdata är från höger till vänster.|
| [line_weight](/cells/sv/python-net/aspose.cells.charts/sparklinegroup/line_weight) | Hämtar och ställer in linjevikten i varje linje sparkline i sparklinegruppen, i enheten för poäng.|
| [horizontal_axis_color](/cells/sv/python-net/aspose.cells.charts/sparklinegroup/horizontal_axis_color) | Hämtar och ställer in färgen på den horisontella axeln i sparklinegruppen.|
| [show_horizontal_axis](/cells/sv/python-net/aspose.cells.charts/sparklinegroup/show_horizontal_axis) | Indikerar om sparklinjens horisontella axel ska visas.<br/> Den horisontella axeln visas om gnistlinjen har data som korsar nollaxeln.|
| [horizontal_axis_date_range](/cells/sv/python-net/aspose.cells.charts/sparklinegroup/horizontal_axis_date_range) | Representerar intervallet som innehåller datumvärdena för sparklinedata.|
| [vertical_axis_max_value_type](/cells/sv/python-net/aspose.cells.charts/sparklinegroup/vertical_axis_max_value_type) | Representerar den vertikala axelns maximala värdetyp.|
| [vertical_axis_max_value](/cells/sv/python-net/aspose.cells.charts/sparklinegroup/vertical_axis_max_value) | Hämtar och ställer in det anpassade maxvärdet för den vertikala axeln.|
| [vertical_axis_min_value_type](/cells/sv/python-net/aspose.cells.charts/sparklinegroup/vertical_axis_min_value_type) | Representerar den vertikala axelns minimivärdestyp.|
| [vertical_axis_min_value](/cells/sv/python-net/aspose.cells.charts/sparklinegroup/vertical_axis_min_value) | Hämtar och ställer in det anpassade minimivärdet för den vertikala axeln.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [reset_ranges(data_range, is_vertical, location_range)](/cells/sv/python-net/aspose.cells.charts/sparklinegroup/reset_ranges/#str-bool-CellArea) |Återställer dataintervallet och platsintervallet för sparklinegruppen.<br/> Den här metoden kommer att rensa ursprungliga sparkline-objekt i gruppen och skapar nya sparkline-objekt för de nya serierna.|



###  Exempel

```python
from aspose.cells import CellArea, SaveFormat, Workbook
from aspose.cells.charts import SparklineType
from aspose.pydrawing import Color

book = Workbook()
sheet = book.worksheets[0]
sheet.cells.get("A1").put_value(5)
sheet.cells.get("B1").put_value(2)
sheet.cells.get("C1").put_value(1)
sheet.cells.get("D1").put_value(3)
#  Define the CellArea
ca = CellArea()
ca.start_column = 4
ca.end_column = 4
ca.start_row = 0
ca.end_row = 0
idx = sheet.sparkline_group_collection.add(SparklineType.LINE, "A1:D1", False, ca)
group = sheet.sparkline_group_collection[idx]
group.sparkline_collection.add(sheet.name + "!A1:D1", 0, 4)
#  Create CellsColor
clr = book.create_cells_color()
clr.color = Color.orange
group.series_color = clr
#  set the high points are colored green and the low points are colored red
group.show_high_point = True
group.show_low_point = True
group.high_point_color.color = Color.green
group.low_point_color.color = Color.red
#  set line weight
group.line_weight = 1.0
book.save("output.xlsx", SaveFormat.XLSX)

```

###  Se även
* modul [aspose.cells.charts](..)
* klass [Sparkline](/cells/sv/python-net/aspose.cells.charts/sparkline)
