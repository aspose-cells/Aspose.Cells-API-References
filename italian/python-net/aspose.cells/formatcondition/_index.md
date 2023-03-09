---
title: classe FormatCondition
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 690
url: /it/python-net/aspose.cells/formatcondition/
is_root: false
---
##  classe FormatCondition
Rappresenta la condizione di formattazione condizionale.



Il tipo FormatCondition espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [formula1](/cells/it/python-net/aspose.cells/formatcondition/formula1) | Ottiene e imposta il valore o l'espressione associati alla formattazione condizionale.|
| [formula2](/cells/it/python-net/aspose.cells/formatcondition/formula2) | Ottiene e imposta il valore o l'espressione associati alla formattazione condizionale.|
| [operator](/cells/it/python-net/aspose.cells/formatcondition/operator) | Ottiene e imposta il tipo di operatore di formato condizionale.|
| [stop_if_true](/cells/it/python-net/aspose.cells/formatcondition/stop_if_true) | True, nessuna regola con priorità inferiore può essere applicata a questa regola, quando questa regola restituisce true.<br/> Si applica solo a Excel 2007;|
| [priority](/cells/it/python-net/aspose.cells/formatcondition/priority) | La priorità di questa regola di formattazione condizionale. Questo valore viene utilizzato per determinare quale<br/>il formato deve essere valutato e reso. I valori numerici inferiori hanno una priorità maggiore di<br/> valori numerici più alti, dove '1' è la priorità più alta.|
| [style](/cells/it/python-net/aspose.cells/formatcondition/style) | Ottiene o imposta lo stile degli intervalli di celle formattati condizionali.|
| [type](/cells/it/python-net/aspose.cells/formatcondition/type) | Ottiene e imposta se il formato condizionale Type.|
| [icon_set](/cells/it/python-net/aspose.cells/formatcondition/icon_set) | Ottieni l'istanza "IconSet" della formattazione condizionale.<br/>IconSetType dell'istanza predefinita è TrafficLights31.<br/> Valido solo per type = IconSet.|
| [data_bar](/cells/it/python-net/aspose.cells/formatcondition/data_bar) | Ottieni l'istanza "DataBar" della formattazione condizionale.<br/>Il colore dell'istanza predefinita è il blu.<br/> Valido solo per il tipo è DataBar.|
| [color_scale](/cells/it/python-net/aspose.cells/formatcondition/color_scale) |Ottieni l'istanza "ColorScale" della formattazione condizionale.<br/>L'istanza predefinita è un 3ColorScale "verde-giallo-rosso".<br/> Valido solo per type = ColorScale.|
| [top10](/cells/it/python-net/aspose.cells/formatcondition/top10) | Ottieni l'istanza "Top10" della formattazione condizionale.<br/>La regola dell'istanza predefinita evidenzia le celle cui<br/>i valori rientrano nella fascia dei primi 10.<br/> Valido solo per il tipo è Top10.|
| [above_average](/cells/it/python-net/aspose.cells/formatcondition/above_average) | Ottieni l'istanza "AboveAverage" della formattazione condizionale.<br/> La regola dell'istanza predefinita evidenzia le celle che sono<br/>sopra la media per tutti i valori nell'intervallo.<br/> Valido solo per tipo = Sopra la media.|
| [text](/cells/it/python-net/aspose.cells/formatcondition/text) | Il valore del testo in una regola di formattazione condizionale "il testo contiene".<br/>Valido solo per type = containsText, notContainsText, BeginWith e EndsWith.<br/> Il valore predefinito è nullo.|
| [time_period](/cells/it/python-net/aspose.cells/formatcondition/time_period) | Il periodo di tempo applicabile in una regola di formattazione condizionale "data in cui si verifica...".<br/>Valido solo per type = timePeriod.<br/> Il valore predefinito è TimePeriodType.Today.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [get_formula1(is_r1c1, is_local)](/cells/it/python-net/aspose.cells/formatcondition/get_formula1/#bool-bool) | Ottiene il valore o l'espressione associati a questa condizione di formato.|
| [get_formula1(is_r1c1, is_local, row, column)](/cells/it/python-net/aspose.cells/formatcondition/get_formula1/#bool-bool-int-int) |Ottiene il valore o l'espressione della formattazione condizionale della cella.|
| [get_formula1(row, column)](/cells/it/python-net/aspose.cells/formatcondition/get_formula1/#int-int) | Ottiene la formula della formattazione condizionale della cella.|
| [get_formula2(is_r1c1, is_local)](/cells/it/python-net/aspose.cells/formatcondition/get_formula2/#bool-bool) | Ottiene il valore o l'espressione associati a questa condizione di formato.|
| [get_formula2(is_r1c1, is_local, row, column)](/cells/it/python-net/aspose.cells/formatcondition/get_formula2/#bool-bool-int-int) |Ottiene il valore o l'espressione della formattazione condizionale della cella.|
| [get_formula2(row, column)](/cells/it/python-net/aspose.cells/formatcondition/get_formula2/#int-int) | Ottiene la formula della formattazione condizionale della cella.|
| [set_formulas(formula1, formula2, is_r1c1, is_local)](/cells/it/python-net/aspose.cells/formatcondition/set_formulas/#str-str-bool-bool) | Imposta il valore o l'espressione associati a questa condizione di formato.|
| [set_formula1(formula, is_r1c1, is_local)](/cells/it/python-net/aspose.cells/formatcondition/set_formula1/#str-bool-bool) | Imposta il valore o l'espressione associati a questa condizione di formato.|
| [set_formula2(formula, is_r1c1, is_local)](/cells/it/python-net/aspose.cells/formatcondition/set_formula2/#str-bool-bool) | Imposta il valore o l'espressione associati a questa condizione di formato.|



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
