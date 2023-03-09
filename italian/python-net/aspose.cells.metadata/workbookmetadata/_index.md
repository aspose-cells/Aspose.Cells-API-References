---
title: classe WorkbookMetadata
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 20
url: /it/python-net/aspose.cells.metadata/workbookmetadata/
is_root: false
---
##  classe WorkbookMetadata
Rappresenta i metadati.



Il tipo WorkbookMetadata espone i membri seguenti:

###  Costruttori
| Costruttore| Descrizione|
| :- | :- |
| [WorkbookMetadata(file_name, options)](/cells/it/python-net/aspose.cells.metadata/workbookmetadata/__init__/#str-MetadataOptions) | Creare l'oggetto dei metadati.|
| [WorkbookMetadata(stream, options)](/cells/it/python-net/aspose.cells.metadata/workbookmetadata/__init__/#io.RawIOBase-MetadataOptions) | Creare l'oggetto dei metadati.|


###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [options](/cells/it/python-net/aspose.cells.metadata/workbookmetadata/options) | Ottiene le opzioni dei metadati.|
| [built_in_document_properties](/cells/it/python-net/aspose.cells.metadata/workbookmetadata/built_in_document_properties) |Restituisce una raccolta [DocumentProperty](/cells/it/python-net/aspose.cells.properties/documentproperty) che rappresenta tutte le proprietà del documento predefinite del foglio di calcolo.|
| [custom_document_properties](/cells/it/python-net/aspose.cells.metadata/workbookmetadata/custom_document_properties) | Restituisce una raccolta [DocumentProperty](/cells/it/python-net/aspose.cells.properties/documentproperty) che rappresenta tutte le proprietà del documento personalizzato del foglio di calcolo.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [save(file_name)](/cells/it/python-net/aspose.cells.metadata/workbookmetadata/save/#str) | Salva i metadati modificati nel file.|
| [save(stream)](/cells/it/python-net/aspose.cells.metadata/workbookmetadata/save/#io.RawIOBase) | Salva i metadati modificati nello stream.|



###  Esempi

L'esempio seguente crea un WorkbookMetadata.

```python
from aspose.cells.metadata import MetadataOptions, MetadataType, WorkbookMetadata

options = MetadataOptions(MetadataType.DOCUMENT_PROPERTIES)
meta = WorkbookMetadata("book1.xlsx", options)
meta.custom_document_properties.add("test", "test")
meta.save("book2.xlsx")

```

###  Guarda anche
* modulo [aspose.cells.metadata](..)
* classe [DocumentProperty](/cells/it/python-net/aspose.cells.properties/documentproperty)
