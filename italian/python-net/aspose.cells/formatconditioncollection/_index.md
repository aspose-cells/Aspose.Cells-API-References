---
title: classe FormatConditionCollection
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 700
url: /it/python-net/aspose.cells/formatconditioncollection/
is_root: false
---
##  classe FormatConditionCollection
Rappresenta la formattazione condizionale.
FormatConditions può contenere fino a tre formati condizionali.



Il tipo FormatConditionCollection espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [count](/cells/it/python-net/aspose.cells/formatconditioncollection/count) | Ottiene il conteggio delle condizioni.|
| [range_count](/cells/it/python-net/aspose.cells/formatconditioncollection/range_count) | Ottiene il conteggio degli intervalli con formattazione condizionale.|



Ottiene la condizione di formattazione per indice.
###  Indicizzatore
| Nome| Descrizione|
| :- | :- |
| [index] | l'indice della condizione di formattazione da restituire.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [add_condition(type, operator_type, formula1, formula2)](/cells/it/python-net/aspose.cells/formatconditioncollection/add_condition/#FormatConditionType-OperatorType-str-str) | Aggiunge una condizione di formattazione.|
| [add_condition(type)](/cells/it/python-net/aspose.cells/formatconditioncollection/add_condition/#FormatConditionType) | Aggiungi una condizione di formato.|
| [remove_area(index)](/cells/it/python-net/aspose.cells/formatconditioncollection/remove_area/#int) | Rimuove l'intervallo di celle formattato condizionale per indice.|
| [remove_area(start_row, start_column, total_rows, total_columns)](/cells/it/python-net/aspose.cells/formatconditioncollection/remove_area/#int-int-int-int) | Rimuovi la formattazione condizionale nell'intervallo.|
| [add(cell_area, type, operator_type, formula1, formula2)](/cells/it/python-net/aspose.cells/formatconditioncollection/add/#CellArea-FormatConditionType-OperatorType-str-str) | Aggiunge una condizione di formattazione e un numero di celle interessate a FormatConditions<br/>FormatConditions può contenere fino a tre formati condizionali.<br/> Nelle formule di formattazione condizionale non sono ammessi riferimenti agli altri fogli.|
| [add_area(cell_area)](/cells/it/python-net/aspose.cells/formatconditioncollection/add_area/#CellArea) | Aggiunge un intervallo di celle formattato condizionale.|
| [get_cell_area(index)](/cells/it/python-net/aspose.cells/formatconditioncollection/get_cell_area/#int) | Ottiene l'intervallo di celle formattato condizionale in base all'indice.|
| [remove_condition(index)](/cells/it/python-net/aspose.cells/formatconditioncollection/remove_condition/#int) | Rimuove la condizione di formattazione per indice.|



###  Esempio

```python
from aspose.cells import CellArea, FormatConditionType, OperatorType, Workbook
from aspose.pydrawing import Color

# Create a new Workbook.
workbook = Workbook()
# Get the first worksheet.
sheet = workbook.worksheets[0]
# Adds an empty conditional formatting
index = sheet.conditional_formattings.add()
fcs = sheet.conditional_formattings[index]
# Sets the conditional format range.
ca = CellArea()
ca.start_row = 0
ca.end_row = 0
ca.start_column = 0
ca.end_column = 0
fcs.add_area(ca)
ca = CellArea()
ca.start_row = 1
ca.end_row = 1
ca.start_column = 1
ca.end_column = 1
fcs.add_area(ca)
# Adds condition.
conditionIndex = fcs.add_condition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "=A2", "100")
# Adds condition.
conditionIndex2 = fcs.add_condition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "50", "100")
# Sets the background color.
fc = fcs[conditionIndex]
fc.style.background_color = Color.red
# Saving the Excel file
workbook.save("output.xls")

```

###  Guarda anche
* modulo [aspose.cells](..)
