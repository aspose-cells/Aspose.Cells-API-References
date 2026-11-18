---
title: "WorkbookRender klass"
linktitle: "WorkbookRender"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "WorkbookRender klass. Inkapslar objektet som representerar workbookrender i Go."
type: docs
weight: 200
url: /sv/go-cpp/workbookrender/
---

## WorkbookRender class

Representerar en arbetsboksrendering. Konstruktorn för denna klass måste användas efter ändring av sidinställningar och cellstil.

```go

type WorkbookRender struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewWorkbookRender](./newworkbookrender/) | Konstruktionen av WorkbookRender |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetPageCount](./getpagecount/) | Hämtar det totala sidantalet för workbook. |
| [GetPageSizeInch](./getpagesizeinch/) | Hämta sidstorlek i tum för utdatabilden. |
| [ToImage](./toimage/) | Rendera hela arbetsboken som Tiff-bild till ström. |
| [ToImage_String](./toimage_string/) | Rendera hela arbetsboken som Tiff-bild till en fil. |
| [ToImage_Int_String](./toimage_int_string/) | Rendera en viss sida till en fil. |
| [ToImage_Int](./toimage_int/) | Rendera en viss sida till en ström. |
| [Dispose](./dispose/) | Frigör resurser som skapats och används för rendering. |
