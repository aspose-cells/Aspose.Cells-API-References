---
title: classe ChartArea
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 40
url: /it/python-net/aspose.cells.charts/chartarea/
is_root: false
---
##  classe ChartArea
Incapsula l'oggetto che rappresenta l'area del grafico nel foglio di lavoro.



**Eredità:** [ChartArea](/cells/python-net/aspose.cells.charts/chartarea) → 
[ChartFrame](/cells/it/python-net/aspose.cells.charts/chartframe)



Il tipo ChartArea espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [is_inner_mode](/cells/it/python-net/aspose.cells.charts/chartarea/is_inner_mode) | Indica se la dimensione dell'area del tracciato include i segni di graduazione e le etichette degli assi.<br/> False specifica che la dimensione determinerà la dimensione dell'area del tracciato, i segni di graduazione e le etichette degli assi.|
| [border](/cells/it/python-net/aspose.cells.charts/chartarea/border) | Ottiene lo [Line](/cells/it/python-net/aspose.cells.drawing/line).|
| [area](/cells/it/python-net/aspose.cells.charts/chartarea/area) | Ottiene lo [ChartFrame.area](/cells/it/python-net/aspose.cells.charts/chartframe#area).|
| [text_font](/cells/it/python-net/aspose.cells.charts/chartarea/text_font) | Ottiene un oggetto [ChartFrame.font](/cells/it/python-net/aspose.cells.charts/chartframe#font) dell'oggetto ChartFrame specificato.|
| [text_options](/cells/it/python-net/aspose.cells.charts/chartarea/text_options) | Ottiene e imposta le opzioni del testo.|
| [font](/cells/it/python-net/aspose.cells.charts/chartarea/font) | Ottiene un oggetto [ChartArea.font](/cells/it/python-net/aspose.cells.charts/chartarea#font) dell'oggetto chartarea specificato.|
| [auto_scale_font](/cells/it/python-net/aspose.cells.charts/chartarea/auto_scale_font) | True se il testo nell'oggetto cambia la dimensione del carattere quando cambia la dimensione dell'oggetto.|
| [background_mode](/cells/it/python-net/aspose.cells.charts/chartarea/background_mode) | Ottiene e imposta la modalità di visualizzazione dello sfondo|
| [background](/cells/it/python-net/aspose.cells.charts/chartarea/background) | Ottiene e imposta la modalità di visualizzazione dello sfondo|
| [is_automatic_size](/cells/it/python-net/aspose.cells.charts/chartarea/is_automatic_size) | Indica se la cornice del grafico è ridimensionata automaticamente.|
| [x](/cells/it/python-net/aspose.cells.charts/chartarea/x) | Ottiene o ottiene l'offset orizzontale dalla colonna nell'angolo superiore sinistro.|
| [y](/cells/it/python-net/aspose.cells.charts/chartarea/y) |Ottiene o ottiene l'offset verticale dalla riga dell'angolo superiore sinistro.|
| [height](/cells/it/python-net/aspose.cells.charts/chartarea/height) | Ottiene o imposta l'offset verticale dalla relativa riga nell'angolo inferiore destro.|
| [width](/cells/it/python-net/aspose.cells.charts/chartarea/width) | Ottiene o imposta l'offset orizzontale dalla colonna nell'angolo inferiore destro.|
| [shadow](/cells/it/python-net/aspose.cells.charts/chartarea/shadow) | Vero se la cornice ha un'ombra.|
| [shape_properties](/cells/it/python-net/aspose.cells.charts/chartarea/shape_properties) | Ottiene l'oggetto [ChartFrame.shape_properties](/cells/it/python-net/aspose.cells.charts/chartframe#shape_properties).|
| [is_default_pos_be_set](/cells/it/python-net/aspose.cells.charts/chartarea/is_default_pos_be_set) | Indica se la posizione predefinita (DefaultX, DefaultY, DefaultWidth e DefaultHeight) è impostata.|
| [default_x](/cells/it/python-net/aspose.cells.charts/chartarea/default_x) | Rappresenta x della posizione predefinita|
| [default_y](/cells/it/python-net/aspose.cells.charts/chartarea/default_y) | Rappresenta y della posizione predefinita|
| [default_width](/cells/it/python-net/aspose.cells.charts/chartarea/default_width) | Rappresenta la larghezza della posizione predefinita|
| [default_height](/cells/it/python-net/aspose.cells.charts/chartarea/default_height) | Rappresenta l'altezza della posizione predefinita|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [set_position_auto()](/cells/it/python-net/aspose.cells.charts/chartarea/set_position_auto/#) | Imposta la posizione della cornice su automatico|



###  Esempi

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

###  Guarda anche
* modulo [aspose.cells.charts](..)
* classe [ChartArea](/cells/it/python-net/aspose.cells.charts/chartarea)
* classe [ChartFrame](/cells/it/python-net/aspose.cells.charts/chartframe)
* classe [Line](/cells/it/python-net/aspose.cells.drawing/line)
