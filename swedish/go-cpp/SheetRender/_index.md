---
title: "SheetRender-klass"
linktitle: "SheetRender"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "SheetRender-klass. Inkapslar objektet som representerar sheetrender i Go."
type: docs
weight: 200
url: /sv/go-cpp/sheetrender/
---

## SheetRender class

Representerar en arbetsbladsrendering som kan rendera arbetsblad till olika bilder såsom (BMP, PNG, JPEG, TIFF…). Konstruktorn för denna klass måste användas efter ändring av sidinställningar och cellstil.

```go

type SheetRender struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewSheetRender](./newsheetrender/) | konstruktionen av SheetRender, kräver arbetsblad och ImageOrPrintOptions som parametrar |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetPageCount](./getpagecount/) | Hämtar det totala sidantalet för det aktuella arbetsbladet. |
| [GetPageScale](./getpagescale/) | Hämtar den beräknade sidskalan för bladet. Returnerar den inställda skalan om PageSetup.Zoom är satt. Annars returneras den beräknade skalan enligt PageSetup.FitToPagesWide och PageSetup.FitToPagesTall. |
| [GetPageSizeInch](./getpagesizeinch/) | Hämta sidstorlek i tum för utdatabilden. |
| [ToImage_Int_String](./toimage_int_string/) | Rendera en viss sida till en fil. |
| [ToImage_Int](./toimage_int/) | Rendera en viss sida till en ström. |
| [ToTiff](./totiff/) | Rendera hela arbetsbladet som Tiff-bild till en ström. |
| [ToTiff_String](./totiff_string/) | Rendera hela arbetsbladet som Tiff-bild till en fil. |
| [Dispose](./dispose/) | Frigör resurser som skapats och används för rendering. |
