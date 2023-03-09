---
title: classe IconSet
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 900
url: /it/python-net/aspose.cells/iconset/
is_root: false
---
##  classe IconSet
 Descrivi la regola di formattazione condizionale IconSet.
Questa regola di formattazione condizionale applica le icone alle celle
secondo i loro valori.



Il tipo IconSet espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [cf_icons](/cells/it/python-net/aspose.cells/iconset/cf_icons) | Prendi il [ConditionalFormattingIcon](/cells/it/python-net/aspose.cells/conditionalformattingicon) dalla collezione|
| [cfvos](/cells/it/python-net/aspose.cells/iconset/cfvos) | Ottenere l'istanza CFValueObjects.|
| [type](/cells/it/python-net/aspose.cells/iconset/type) | Ottenere o impostare il tipo di set di icone da visualizzare.<br/>L'impostazione del tipo controllerà automaticamente se il conteggio di Cfvos corrente è<br/> accordo con il nuovo tipo.Se non accordo, i vecchi Cfvo saranno puliti e<br/> verranno aggiunti Cfvo predefiniti.|
| [is_custom](/cells/it/python-net/aspose.cells/iconset/is_custom) | Indica se il set di icone è personalizzato.<br/> Il valore predefinito è false.|
| [show_value](/cells/it/python-net/aspose.cells/iconset/show_value) | Ottieni o imposta il flag che indica se mostrare i valori delle celle su cui è applicato questo set di icone.<br/> Il valore predefinito è vero.|
| [reverse](/cells/it/python-net/aspose.cells/iconset/reverse) | Ottieni o imposta il flag che indica se invertire l'ordine predefinito delle icone in questo set di icone.<br/> Il valore predefinito è false.|



###  Esempi

```python
from aspose.cells import CellArea, FormatConditionType, IconSetType, Workbook

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
idx = fcs.add_condition(FormatConditionType.ICON_SET)
fcs.add_area(ca)
cond = fcs[idx]
# Get Icon Set
iconSet = cond.icon_set
# Set Icon Type
iconSet.type = IconSetType.ARROWS3
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
* classe [ConditionalFormattingIcon](/cells/it/python-net/aspose.cells/conditionalformattingicon)
