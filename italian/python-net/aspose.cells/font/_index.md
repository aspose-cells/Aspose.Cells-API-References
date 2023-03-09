---
title: classe Font
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 650
url: /it/python-net/aspose.cells/font/
is_root: false
---
##  classe Font
Incapsula l'oggetto font utilizzato in un foglio di calcolo.



Il tipo Font espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [charset](/cells/it/python-net/aspose.cells/font/charset) | Rappresenta il set di caratteri.|
| [is_italic](/cells/it/python-net/aspose.cells/font/is_italic) | Ottiene o imposta un valore che indica se il tipo di carattere è corsivo.|
| [is_bold](/cells/it/python-net/aspose.cells/font/is_bold) |Ottiene o imposta un valore che indica se il tipo di carattere è in grassetto.|
| [caps_type](/cells/it/python-net/aspose.cells/font/caps_type) | Ottiene e imposta il tipo di maiuscole di testo.|
| [strike_type](/cells/it/python-net/aspose.cells/font/strike_type) | Ottiene il tipo di avvertimento del testo.|
| [is_strikeout](/cells/it/python-net/aspose.cells/font/is_strikeout) | Ottiene o imposta un valore che indica se il tipo di carattere è barrato singolo.|
| [script_offset](/cells/it/python-net/aspose.cells/font/script_offset) | Ottiene e imposta l'offset dello script, in unità di percentuale|
| [is_superscript](/cells/it/python-net/aspose.cells/font/is_superscript) | Ottiene o imposta un valore che indica se il tipo di carattere è super script.|
| [is_subscript](/cells/it/python-net/aspose.cells/font/is_subscript) | Ottiene o imposta un valore che indica se il tipo di carattere è pedice.|
| [underline](/cells/it/python-net/aspose.cells/font/underline) | Ottiene o imposta il tipo di sottolineatura del carattere.|
| [name](/cells/it/python-net/aspose.cells/font/name) | Ottiene o imposta il nome dell'oggetto [Font](/cells/it/python-net/aspose.cells/font).|
| [double_size](/cells/it/python-net/aspose.cells/font/double_size) | Ottiene e imposta la doppia dimensione del carattere.|
| [size](/cells/it/python-net/aspose.cells/font/size) | Ottiene o imposta la dimensione del carattere.|
| [theme_color](/cells/it/python-net/aspose.cells/font/theme_color) | Ottiene e imposta il colore del tema.|
| [color](/cells/it/python-net/aspose.cells/font/color) | Ottiene o imposta il colore del tipo di carattere.|
| [argb_color](/cells/it/python-net/aspose.cells/font/argb_color) | Ottiene e imposta il colore con un valore ARGB a 32 bit.|
| [is_normalize_heights](/cells/it/python-net/aspose.cells/font/is_normalize_heights) | Indica se eseguire la normalizzazione dell'altezza da applicare al testo.|
| [scheme_type](/cells/it/python-net/aspose.cells/font/scheme_type) | Ottiene e imposta il tipo di schema del carattere.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [equals(font)](/cells/it/python-net/aspose.cells/font/equals/#Font) | Controlla se due caratteri sono uguali.|



###  Esempi

```python
from aspose.cells import Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[0]
# Accessing the "A1" cell from the worksheet
cell = worksheet.cells.get("A1")
# Adding some value to the "A1" cell
cell.put_value("Hello Aspose!")
font = cell.get_style().font
# Setting the font name to "Times New Roman"
font.name = "Times New Roman"
# Setting font size to 14
font.size = 14
# setting font color as Red
font.color = Color.red
# Saving the Excel file
workbook.save(r"dest.xls")

```

###  Guarda anche
* modulo [aspose.cells](..)
* classe [Font](/cells/it/python-net/aspose.cells/font)
