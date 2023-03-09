---
title: classe HorizontalPageBreak
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 750
url: /it/python-net/aspose.cells/horizontalpagebreak/
is_root: false
---
##  classe HorizontalPageBreak
Incapsula l'oggetto che rappresenta un'interruzione di pagina orizzontale.



Il tipo HorizontalPageBreak espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [start_column](/cells/it/python-net/aspose.cells/horizontalpagebreak/start_column) | Ottiene l'indice di colonna iniziale di questa interruzione di pagina orizzontale.|
| [end_column](/cells/it/python-net/aspose.cells/horizontalpagebreak/end_column) |Ottiene l'indice di colonna finale di questa interruzione di pagina orizzontale.|
| [row](/cells/it/python-net/aspose.cells/horizontalpagebreak/row) | Ottiene l'indice di riga in base zero.|



###  Esempio

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[0]
# Add a page break at cell Y30
Index = worksheet.horizontal_page_breaks.add("Y30")
# get the newly added horizontal page break
hPageBreak = worksheet.horizontal_page_breaks[Index]

```

###  Guarda anche
* modulo [aspose.cells](..)
