---
title: classe Top10
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 1480
url: /it/python-net/aspose.cells/top10/
is_root: false
---
##  classe Top10
 Descrivi la regola di formattazione condizionale Top10.
Questa regola di formattazione condizionale evidenzia le celle cui
i valori rientrano nella parentesi N superiore o N inferiore, come specificato.



Il tipo Top10 espone i membri seguenti:

###  Costruttori
| Costruttore| Descrizione|
| :- | :- |
| [Top10()](/cells/it/python-net/aspose.cells/top10/__init__/#) |Costruisce una nuova istanza di Top10|


###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [is_percent](/cells/it/python-net/aspose.cells/top10/is_percent) | Ottenere o impostare se una regola "top/bottom n" è una regola "top/bottom n percent".<br/> Il valore predefinito è false.|
| [is_bottom](/cells/it/python-net/aspose.cells/top10/is_bottom) | Ottieni o imposta se una regola "top/bottom n" è una regola "bottom n".<br/> Il valore predefinito è false.|
| [rank](/cells/it/python-net/aspose.cells/top10/rank) | Ottieni o imposta il valore di "n" in una regola di formattazione condizionale "n superiore/inferiore".<br/>Se IsPercent è vero, il valore deve essere compreso tra 0 e 100.<br/>Altrimenti deve essere compreso tra 0 e 1000.<br/> Il valore predefinito è 10.|



###  Esempio

```python
from aspose.cells import CellArea, FormatConditionType, OperatorType, Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
sheet = workbook.worksheets[0]
# Adds an empty conditional formatting
index = sheet.conditional_formattings.add()
fcs = sheet.conditional_formattings[index]
# Sets the conditional format range.
ca = CellArea.create_cell_area(0, 0, 10, 10)
fcs.add_area(ca)
# Adds condition.
conditionIndex = fcs.add_condition(FormatConditionType.TOP10, OperatorType.NONE, None, None)
# Sets the background color.
fc = fcs[conditionIndex]
fc.style.background_color = Color.red
top10 = fc.top10
# Set the Top N
top10.rank = 5
# Saving the Excel file
workbook.save("output.xls")

```

###  Guarda anche
* modulo [aspose.cells](..)
