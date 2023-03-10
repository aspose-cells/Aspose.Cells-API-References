---
title: classe ExternalLink
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 560
url: /it/python-net/aspose.cells/externallink/
is_root: false
---
##  classe ExternalLink
Rappresenta un collegamento esterno in una cartella di lavoro.



Il tipo ExternalLink espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [type](/cells/it/python-net/aspose.cells/externallink/type) | Ottiene il tipo di collegamento esterno.|
| [original_data_source](/cells/it/python-net/aspose.cells/externallink/original_data_source) | Rappresenta l'origine dati archiviata del collegamento esterno.|
| [data_source](/cells/it/python-net/aspose.cells/externallink/data_source) | Rappresenta l'origine dati del collegamento esterno.|
| [is_referred](/cells/it/python-net/aspose.cells/externallink/is_referred) | Indica se questo collegamento esterno è referenziato da altri.|
| [is_visible](/cells/it/python-net/aspose.cells/externallink/is_visible) | Indica se questo collegamento esterno è visibile in MS Excel.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [add_external_name(text, refer_to)](/cells/it/python-net/aspose.cells/externallink/add_external_name/#str-str) | Aggiunge un nome esterno.|



###  Esempio

```python
from aspose.cells import Workbook

# Open a file with external links
workbook = Workbook("book1.xls")
# Get External Link
externalLink = workbook.worksheets.external_links[0]
# Change External Link's Data Source
externalLink.data_source = "d:\\link.xls"

```

###  Guarda anche
* modulo [aspose.cells](..)
