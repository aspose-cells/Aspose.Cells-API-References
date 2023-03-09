---
title: classe QueryTable
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 1230
url: /it/python-net/aspose.cells/querytable/
is_root: false
---
##  classe QueryTable
Rappresenta le informazioni QueryTable.



Il tipo QueryTable espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [connection_id](/cells/it/python-net/aspose.cells/querytable/connection_id) | Ottiene l'ID connessione della tabella di query.|
| [external_connection](/cells/it/python-net/aspose.cells/querytable/external_connection) | Ottiene la connessione esterna correlata.|
| [name](/cells/it/python-net/aspose.cells/querytable/name) | Ottiene il nome di querytable.|
| [result_range](/cells/it/python-net/aspose.cells/querytable/result_range) | Ottiene l'intervallo del risultato.|
| [preserve_formatting](/cells/it/python-net/aspose.cells/querytable/preserve_formatting) | Restituisce o imposta PreserveFormatting dell'oggetto.|
| [adjust_column_width](/cells/it/python-net/aspose.cells/querytable/adjust_column_width) | Restituisce o imposta l'oggetto AdjustColumnWidth dell'oggetto.|



###  Esempio

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the first worksheet
worksheet = workbook.worksheets[0]
# Getting the first query table in the worksheet
qt = worksheet.query_tables[0]
# Getting display address of the query table.
address = qt.result_range.address

```

###  Guarda anche
* modulo [aspose.cells](..)
