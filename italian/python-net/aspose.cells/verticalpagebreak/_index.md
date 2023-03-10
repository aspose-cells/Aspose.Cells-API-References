---
title: classe VerticalPageBreak
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 1560
url: /it/python-net/aspose.cells/verticalpagebreak/
is_root: false
---
##  classe VerticalPageBreak
Incapsula l'oggetto che rappresenta un'interruzione di pagina verticale.



Il tipo VerticalPageBreak espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [start_row](/cells/it/python-net/aspose.cells/verticalpagebreak/start_row) | Ottiene l'indice della riga iniziale dell'interruzione di pagina verticale.|
| [end_row](/cells/it/python-net/aspose.cells/verticalpagebreak/end_row) | Ottiene l'indice di riga finale dell'interruzione di pagina verticale.|
| [column](/cells/it/python-net/aspose.cells/verticalpagebreak/column) | Ottiene l'indice di colonna dell'interruzione di pagina verticale.|



###  Esempio

```python
from aspose.cells import Workbook

excel = Workbook()
# Add a pagebreak at G5
excel.worksheets[0].horizontal_page_breaks.add("G5")
excel.worksheets[0].vertical_page_breaks.add("G5")

```

###  Guarda anche
* modulo [aspose.cells](..)
