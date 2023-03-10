---
title: classe Column
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 260
url: /it/python-net/aspose.cells/column/
is_root: false
---
##  classe Column
Rappresenta una singola colonna in un foglio di lavoro.



Il tipo Column espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [index](/cells/it/python-net/aspose.cells/column/index) | Ottiene l'indice di questa colonna.|
| [width](/cells/it/python-net/aspose.cells/column/width) | Ottiene e imposta la larghezza della colonna in unità di caratteri.|
| [group_level](/cells/it/python-net/aspose.cells/column/group_level) |Ottiene il livello di gruppo della colonna.|
| [is_hidden](/cells/it/python-net/aspose.cells/column/is_hidden) | Indica se la colonna è nascosta.|
| [has_custom_style](/cells/it/python-net/aspose.cells/column/has_custom_style) | Indica se questa colonna ha impostazioni di stile personalizzate (diverse da quella predefinita ereditata dalla cartella di lavoro).|
| [style](/cells/it/python-net/aspose.cells/column/style) | Ottiene lo stile di questa colonna.|
| [is_collapsed](/cells/it/python-net/aspose.cells/column/is_collapsed) | se la colonna è collassata|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [apply_style(style, flag)](/cells/it/python-net/aspose.cells/column/apply_style/#Style-StyleFlag) | Applica i formati per un'intera colonna.|
| [get_style()](/cells/it/python-net/aspose.cells/column/get_style/#) | Ottiene lo stile di questa colonna.|
| [set_style(style)](/cells/it/python-net/aspose.cells/column/set_style/#Style) | Imposta lo stile di questa colonna.|



###  Esempio

```python
from aspose.cells import BackgroundType, StyleFlag, Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the first worksheet
worksheet = workbook.worksheets[0]
style = workbook.create_style()
# Setting the background color to Blue
style.background_color = Color.blue
# Setting the foreground color to Red
style.foreground_color = Color.red
# setting Background Pattern
style.pattern = BackgroundType.DIAGONAL_STRIPE
# New Style Flag
styleFlag = StyleFlag()
# Set All Styles
styleFlag.all = True
# Get first Column
column = worksheet.cells.columns[0]
# Apply Style to first Column
column.apply_style(style, styleFlag)
# Saving the Excel file
workbook.save("book1.xls")

```

###  Guarda anche
* modulo [aspose.cells](..)
