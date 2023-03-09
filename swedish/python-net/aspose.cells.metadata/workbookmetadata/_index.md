---
title: WorkbookMetadata klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 20
url: /sv/python-net/aspose.cells.metadata/workbookmetadata/
is_root: false
---
##  WorkbookMetadata klass
Representerar metadata.



Typen WorkbookMetadata avslöjar följande medlemmar:

###  Konstruktörer
| Konstruktör| Beskrivning|
| :- | :- |
| [WorkbookMetadata(file_name, options)](/cells/sv/python-net/aspose.cells.metadata/workbookmetadata/__init__/#str-MetadataOptions) | Skapa metadataobjektet.|
| [WorkbookMetadata(stream, options)](/cells/sv/python-net/aspose.cells.metadata/workbookmetadata/__init__/#io.RawIOBase-MetadataOptions) | Skapa metadataobjektet.|


###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [options](/cells/sv/python-net/aspose.cells.metadata/workbookmetadata/options) | Får alternativen för metadata.|
| [built_in_document_properties](/cells/sv/python-net/aspose.cells.metadata/workbookmetadata/built_in_document_properties) |Returnerar en [DocumentProperty](/cells/sv/python-net/aspose.cells.properties/documentproperty)-samling som representerar alla inbyggda dokumentegenskaper i kalkylarket.|
| [custom_document_properties](/cells/sv/python-net/aspose.cells.metadata/workbookmetadata/custom_document_properties) | Returnerar en [DocumentProperty](/cells/sv/python-net/aspose.cells.properties/documentproperty)-samling som representerar alla anpassade dokumentegenskaper i kalkylarket.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [save(file_name)](/cells/sv/python-net/aspose.cells.metadata/workbookmetadata/save/#str) | Spara den modifierade metadatan i filen.|
| [save(stream)](/cells/sv/python-net/aspose.cells.metadata/workbookmetadata/save/#io.RawIOBase) | Spara den modifierade metadatan i strömmen.|



###  Exempel

Följande exempel skapar en WorkbookMetadata.

```python
from aspose.cells.metadata import MetadataOptions, MetadataType, WorkbookMetadata

options = MetadataOptions(MetadataType.DOCUMENT_PROPERTIES)
meta = WorkbookMetadata("book1.xlsx", options)
meta.custom_document_properties.add("test", "test")
meta.save("book2.xlsx")

```

###  Se även
* modul [aspose.cells.metadata](..)
* klass [DocumentProperty](/cells/sv/python-net/aspose.cells.properties/documentproperty)
