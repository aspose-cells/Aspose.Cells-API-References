---
title: classe SparklineGroup
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 280
url: /it/python-net/aspose.cells.charts/sparklinegroup/
is_root: false
---
##  classe SparklineGroup
[Sparkline](/cells/it/python-net/aspose.cells.charts/sparkline) è organizzato in gruppi sparkline.Un SparklineGroup contiene un numero variabile di elementi sparkline.
Un gruppo di grafici sparkline specifica il tipo, le impostazioni di visualizzazione e le impostazioni degli assi per i grafici sparkline.



Il tipo SparklineGroup espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [preset_style](/cells/it/python-net/aspose.cells.charts/sparklinegroup/preset_style) | Ottiene e imposta il tipo di stile preimpostato del gruppo sparkline.|
| [sparkline_collection](/cells/it/python-net/aspose.cells.charts/sparklinegroup/sparkline_collection) | Ottiene la raccolta di oggetti [Sparkline](/cells/it/python-net/aspose.cells.charts/sparkline).|
| [sparklines](/cells/it/python-net/aspose.cells.charts/sparklinegroup/sparklines) | Ottiene la raccolta di oggetti [Sparkline](/cells/it/python-net/aspose.cells.charts/sparkline).|
| [type](/cells/it/python-net/aspose.cells.charts/sparklinegroup/type) | Indica il tipo di grafico sparkline del gruppo di grafici sparkline.|
| [plot_empty_cells_type](/cells/it/python-net/aspose.cells.charts/sparklinegroup/plot_empty_cells_type) | Indica come tracciare le celle vuote.|
| [display_hidden](/cells/it/python-net/aspose.cells.charts/sparklinegroup/display_hidden) |Indica se mostrare i dati in righe e colonne nascoste.|
| [show_high_point](/cells/it/python-net/aspose.cells.charts/sparklinegroup/show_high_point) | Indica se evidenziare i punti più alti dei dati nel gruppo sparkline.|
| [high_point_color](/cells/it/python-net/aspose.cells.charts/sparklinegroup/high_point_color) | Ottiene e imposta il colore dei punti più alti dei dati nel gruppo grafico sparkline.|
| [show_low_point](/cells/it/python-net/aspose.cells.charts/sparklinegroup/show_low_point) | Indica se evidenziare i punti di dati più bassi nel gruppo sparkline.|
| [low_point_color](/cells/it/python-net/aspose.cells.charts/sparklinegroup/low_point_color) | Ottiene e imposta il colore dei punti di dati più bassi nel gruppo sparkline.|
| [show_negative_points](/cells/it/python-net/aspose.cells.charts/sparklinegroup/show_negative_points) | Indica se evidenziare i valori negativi sul gruppo sparkline con un colore o un indicatore diverso.|
| [negative_points_color](/cells/it/python-net/aspose.cells.charts/sparklinegroup/negative_points_color) | Ottiene e imposta il colore dei valori negativi nel gruppo sparkline.|
| [show_first_point](/cells/it/python-net/aspose.cells.charts/sparklinegroup/show_first_point) | Indica se evidenziare il primo punto di dati nel gruppo sparkline.|
| [first_point_color](/cells/it/python-net/aspose.cells.charts/sparklinegroup/first_point_color) | Ottiene e imposta il colore del primo punto di dati nel gruppo sparkline.|
| [show_last_point](/cells/it/python-net/aspose.cells.charts/sparklinegroup/show_last_point) | Indica se evidenziare l'ultimo punto di dati nel gruppo sparkline.|
| [last_point_color](/cells/it/python-net/aspose.cells.charts/sparklinegroup/last_point_color) | Ottiene e imposta il colore dell'ultimo punto di dati nel gruppo sparkline.|
| [show_markers](/cells/it/python-net/aspose.cells.charts/sparklinegroup/show_markers) |Indica se evidenziare ogni punto in ogni sparkline linea nel gruppo sparkline.|
| [markers_color](/cells/it/python-net/aspose.cells.charts/sparklinegroup/markers_color) | Ottiene e imposta il colore dei punti in ogni sparkline di linea nel gruppo di sparkline.|
| [series_color](/cells/it/python-net/aspose.cells.charts/sparklinegroup/series_color) | Ottiene e imposta il colore dei grafici sparkline nel gruppo di grafici sparkline.|
| [plot_right_to_left](/cells/it/python-net/aspose.cells.charts/sparklinegroup/plot_right_to_left) | Indica se i dati del grafico sono da destra a sinistra.|
| [line_weight](/cells/it/python-net/aspose.cells.charts/sparklinegroup/line_weight) | Ottiene e imposta lo spessore della linea in ogni grafico sparkline nel gruppo di grafici sparkline, nell'unità di punti.|
| [horizontal_axis_color](/cells/it/python-net/aspose.cells.charts/sparklinegroup/horizontal_axis_color) | Ottiene e imposta il colore dell'asse orizzontale nel gruppo sparkline.|
| [show_horizontal_axis](/cells/it/python-net/aspose.cells.charts/sparklinegroup/show_horizontal_axis) | Indica se mostrare l'asse orizzontale del grafico sparkline.<br/> L'asse orizzontale viene visualizzato se il grafico sparkline contiene dati che attraversano l'asse zero.|
| [horizontal_axis_date_range](/cells/it/python-net/aspose.cells.charts/sparklinegroup/horizontal_axis_date_range) | Rappresenta l'intervallo che contiene i valori di data per i dati sparkline.|
| [vertical_axis_max_value_type](/cells/it/python-net/aspose.cells.charts/sparklinegroup/vertical_axis_max_value_type) | Rappresenta il tipo di valore massimo dell'asse verticale.|
| [vertical_axis_max_value](/cells/it/python-net/aspose.cells.charts/sparklinegroup/vertical_axis_max_value) | Ottiene e imposta il valore massimo personalizzato per l'asse verticale.|
| [vertical_axis_min_value_type](/cells/it/python-net/aspose.cells.charts/sparklinegroup/vertical_axis_min_value_type) | Rappresenta il tipo di valore minimo dell'asse verticale.|
| [vertical_axis_min_value](/cells/it/python-net/aspose.cells.charts/sparklinegroup/vertical_axis_min_value) | Ottiene e imposta il valore minimo personalizzato per l'asse verticale.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [reset_ranges(data_range, is_vertical, location_range)](/cells/it/python-net/aspose.cells.charts/sparklinegroup/reset_ranges/#str-bool-CellArea) |Reimposta l'intervallo di dati e l'intervallo di posizioni del gruppo sparkline.<br/> Questo metodo cancellerà gli elementi sparkline originali nel gruppo e creerà nuovi elementi sparkline per i nuovi intervalli.|



###  Esempi

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

###  Guarda anche
* modulo [aspose.cells.charts](..)
* classe [Sparkline](/cells/it/python-net/aspose.cells.charts/sparkline)
