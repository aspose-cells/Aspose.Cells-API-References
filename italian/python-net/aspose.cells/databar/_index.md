---
title: classe DataBar
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 400
url: /it/python-net/aspose.cells/databar/
is_root: false
---
##  classe DataBar
 Descrivi la regola di formattazione condizionale DataBar.
Questa regola di formattazione condizionale visualizza un voto
barra dei dati nell'intervallo di celle.



Il tipo DataBar espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [axis_color](/cells/it/python-net/aspose.cells/databar/axis_color) | Ottiene il colore dell'asse per le celle con formattazione condizionale come barre dei dati.|
| [axis_position](/cells/it/python-net/aspose.cells/databar/axis_position) | Ottiene o imposta la posizione dell'asse delle barre dei dati specificata da una regola di formattazione condizionale.|
| [bar_fill_type](/cells/it/python-net/aspose.cells/databar/bar_fill_type) | Ottiene o imposta il modo in cui una barra dei dati viene riempita di colore.|
| [direction](/cells/it/python-net/aspose.cells/databar/direction) |Ottiene o imposta la direzione in cui viene visualizzata la barra dati.|
| [bar_border](/cells/it/python-net/aspose.cells/databar/bar_border) | Ottiene un oggetto che specifica il bordo di una barra dei dati.|
| [negative_bar_format](/cells/it/python-net/aspose.cells/databar/negative_bar_format) | Ottiene l'oggetto NegativeBarFormat associato a una regola di formattazione condizionale della barra dei dati.|
| [min_cfvo](/cells/it/python-net/aspose.cells/databar/min_cfvo) | Ottenere o impostare l'oggetto valore minimo di questo DataBar.<br/> Impossibile impostare null o CFValueObject con tipo FormatConditionValueType.Max su di esso.|
| [max_cfvo](/cells/it/python-net/aspose.cells/databar/max_cfvo) | Ottenere o impostare l'oggetto valore massimo di questo DataBar.<br/> Impossibile impostare null o CFValueObject con tipo FormatConditionValueType.Min.|
| [color](/cells/it/python-net/aspose.cells/databar/color) | Ottieni o imposta questo DataBar's Color.|
| [min_length](/cells/it/python-net/aspose.cells/databar/min_length) | Rappresenta la lunghezza minima della barra dei dati.|
| [max_length](/cells/it/python-net/aspose.cells/databar/max_length) | Rappresenta la lunghezza massima della barra dei dati.|
| [show_value](/cells/it/python-net/aspose.cells/databar/show_value) | Ottieni o imposta il flag che indica se mostrare i valori delle celle su cui è applicata questa barra dati.<br/> Il valore predefinito è vero.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [to_image(cell, img_opts)](/cells/it/python-net/aspose.cells/databar/to_image/#Cell-aspose.cells.rendering.ImageOrPrintOptions) | Visualizza la barra dei dati nella cella nell'array di byte dell'immagine.|



###  Esempi

```python
from aspose.cells import CellArea, DataBarAxisPosition, DataBarBorderType, DataBarFillType, DataBarNegativeColorType, FormatConditionType, FormatConditionValueType, Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
sheet = workbook.worksheets[0]
# Adds an empty conditional formatting
index = sheet.conditional_formattings.add()
fcs = sheet.conditional_formattings[index]
# Sets the conditional format range.
ca = CellArea()
ca.start_row = 0
ca.end_row = 2
ca.start_column = 0
ca.end_column = 0
fcs.add_area(ca)
# Adds condition.
idx = fcs.add_condition(FormatConditionType.DATA_BAR)
fcs.add_area(ca)
cond = fcs[idx]
# Get Databar
dataBar = cond.data_bar
dataBar.color = Color.orange
# Set Databar properties
dataBar.min_cfvo.type = FormatConditionValueType.PERCENTILE
dataBar.min_cfvo.value = 30
dataBar.show_value = False
dataBar.bar_border.type = DataBarBorderType.SOLID
dataBar.bar_border.color = Color.plum
dataBar.bar_fill_type = DataBarFillType.SOLID
dataBar.axis_color = Color.red
dataBar.axis_position = DataBarAxisPosition.MIDPOINT
dataBar.negative_bar_format.color_type = DataBarNegativeColorType.COLOR
dataBar.negative_bar_format.color = Color.white
dataBar.negative_bar_format.border_color_type = DataBarNegativeColorType.COLOR
dataBar.negative_bar_format.border_color = Color.yellow
# Put Cell Values
cell1 = sheet.cells.get("A1")
cell1.put_value(10)
cell2 = sheet.cells.get("A2")
cell2.put_value(120)
cell3 = sheet.cells.get("A3")
cell3.put_value(260)
# Saving the Excel file
workbook.save("book1.xlsx")

```

###  Guarda anche
* modulo [aspose.cells](..)
