---
title: "WorkbookMetadata Class"
linktitle: "WorkbookMetadata"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "WorkbookMetadata‑klass. Inkapslar objektet som representerar workbookmetadata i Go."
type: docs
weight: 200
url: /sv/go-cpp/workbookmetadata/
---

## WorkbookMetadata class

Representerar metadata.

```go

type WorkbookMetadata struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewWorkbookMetadata_String_MetadataOptions](./newworkbookmetadata_string_metadataoptions/) | Skapa metadataobjektet. |
| [NewWorkbookMetadata_Stream_MetadataOptions](./newworkbookmetadata_stream_metadataoptions/) | Skapa metadataobjektet. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetOptions](./getoptions/) | Hämtar alternativen för metadata. |
| [GetBuiltInDocumentProperties](./getbuiltindocumentproperties/) | Returnerar en DocumentProperty-samling som representerar alla inbyggda dokumentegenskaper i kalkylbladet. |
| [GetCustomDocumentProperties](./getcustomdocumentproperties/) | Returnerar en DocumentProperty-samling som representerar alla anpassade dokumentegenskaper i kalkylbladet. |
| [Save_String](./save_string/) | Spara den modifierade metadata till filen. |
| [Save_Stream](./save_stream/) | Spara den modifierade metadata till strömmen. |
