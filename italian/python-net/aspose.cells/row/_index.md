---
title: classe Row
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 1300
url: /it/python-net/aspose.cells/row/
is_root: false
---
##  classe Row
Rappresenta una singola riga in un foglio di lavoro.



Il tipo Row espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [is_blank](/cells/it/python-net/aspose.cells/row/is_blank) | Indica se la riga contiene dati|
| [is_collapsed](/cells/it/python-net/aspose.cells/row/is_collapsed) | se la riga è compressa|
| [height](/cells/it/python-net/aspose.cells/row/height) | Ottiene e imposta l'altezza della riga in unità di punti.|
| [is_hidden](/cells/it/python-net/aspose.cells/row/is_hidden) | Indica se la riga è nascosta.|
| [index](/cells/it/python-net/aspose.cells/row/index) | Ottiene l'indice di questa riga.|
| [group_level](/cells/it/python-net/aspose.cells/row/group_level) | Ottiene il livello di gruppo della riga.|
| [is_height_matched](/cells/it/python-net/aspose.cells/row/is_height_matched) |Indica che l'altezza della riga e l'altezza predefinita del carattere corrispondono.|
| [style](/cells/it/python-net/aspose.cells/row/style) | Rappresenta lo stile di questa riga.|
| [has_custom_style](/cells/it/python-net/aspose.cells/row/has_custom_style) | Indica se questa riga ha impostazioni di stile personalizzate (diverse da quella predefinita ereditata dalla cartella di lavoro).|
| [first_cell](/cells/it/python-net/aspose.cells/row/first_cell) | Ottiene il primo oggetto cella nella riga.|
| [first_data_cell](/cells/it/python-net/aspose.cells/row/first_data_cell) | Ottiene la prima cella non vuota nella riga.|
| [last_cell](/cells/it/python-net/aspose.cells/row/last_cell) | Ottiene l'ultimo oggetto cella nella riga.|
| [last_data_cell](/cells/it/python-net/aspose.cells/row/last_data_cell) | Ottiene l'ultima cella non vuota nella riga.|



Ottiene la cella.
###  Indicizzatore
| Nome| Descrizione|
| :- | :- |
| [index] | L'indice di colonna|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [get_cell_by_index(index)](/cells/it/python-net/aspose.cells/row/get_cell_by_index/#int) | Ottieni la cella per indice specifico nell'elenco.|
| [get_cell_or_null(column)](/cells/it/python-net/aspose.cells/row/get_cell_or_null/#int) | Ottiene la cella o null nell'indice specifico.|
| [get_style()](/cells/it/python-net/aspose.cells/row/get_style/#) | Ottiene lo stile di questa riga.|
| [set_style(style)](/cells/it/python-net/aspose.cells/row/set_style/#Style) | Imposta lo stile di questa riga.|
| [copy_settings(source, check_style)](/cells/it/python-net/aspose.cells/row/copy_settings/#Row-bool) | Copia le impostazioni della riga, come stile, altezza, visibilità, ...ecc.|
| [apply_style(style, flag)](/cells/it/python-net/aspose.cells/row/apply_style/#Style-StyleFlag) | Applica i formati per un'intera riga.|
| [equals(row)](/cells/it/python-net/aspose.cells/row/equals/#Row) | Controlla se questo oggetto fa riferimento alla stessa riga con un altro oggetto riga.|



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
# Get first row
row = worksheet.cells.rows[0]
# Apply Style to first row
row.apply_style(style, styleFlag)
# Saving the Excel file
workbook.save("book1.xls")

```

###  Guarda anche
* modulo [aspose.cells](..)
