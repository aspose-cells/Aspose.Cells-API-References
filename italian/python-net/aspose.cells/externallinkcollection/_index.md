---
title: classe ExternalLinkCollection
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 570
url: /it/python-net/aspose.cells/externallinkcollection/
is_root: false
---
##  classe ExternalLinkCollection
Rappresenta la raccolta di collegamenti esterni in una cartella di lavoro.



Il tipo ExternalLinkCollection espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [count](/cells/it/python-net/aspose.cells/externallinkcollection/count) | Ottiene il numero di elementi effettivamente contenuti nell'insieme.|



Ottiene l'elemento [ExternalLink](/cells/it/python-net/aspose.cells/externallink) in corrispondenza dell'indice specificato.
###  Indicizzatore
| Nome| Descrizione|
| :- | :- |
| [index] | L'indice in base zero dell'elemento.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [add(file_name, sheet_names)](/cells/it/python-net/aspose.cells/externallinkcollection/add/#str-list) | Aggiunge un collegamento esterno.|
| [add(directory_type, file_name, sheet_names)](/cells/it/python-net/aspose.cells/externallinkcollection/add/#DirectoryType-str-list) | Aggiungi un collegamento esterno .|
| [clear()](/cells/it/python-net/aspose.cells/externallinkcollection/clear/#) | Rimuove tutti i link esterni.|
| [clear(update_references_as_local)](/cells/it/python-net/aspose.cells/externallinkcollection/clear/#bool) | Rimuove tutti i link esterni.|
| [remove_at(index)](/cells/it/python-net/aspose.cells/externallinkcollection/remove_at/#int) | Rimuove il collegamento esterno specificato dalla cartella di lavoro.|
| [remove_at(index, update_references_as_local)](/cells/it/python-net/aspose.cells/externallinkcollection/remove_at/#int-bool) | Rimuove il collegamento esterno specificato dalla cartella di lavoro.|



###  Esempio

```python
from aspose.cells import Workbook

# Open a file with external links
workbook = Workbook("book1.xls")
# Change external link data source
workbook.worksheets.external_links[0].data_source = "d:\\link.xls"

```

###  Guarda anche
* modulo [aspose.cells](..)
* classe [ExternalLink](/cells/it/python-net/aspose.cells/externallink)
