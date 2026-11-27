---
title: "Class GridSheetRender"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridDesktop.Data.GridSheetRender class. Representerar en kalkylbladsrendering som kan rendera kalkylblad till olika bilder såsom BMP, PNG, JPEG, TIFF.. Konstruktorn för denna klass måste användas efter modifiering av sidinställningscellstil"
type: docs
url: /sv/net/aspose.cells.griddesktop.data/gridsheetrender/
---
## GridSheetRender class

Representerar en arbetsbladsrendering som kan rendera arbetsblad till olika bilder såsom (BMP, PNG, JPEG, TIFF…). Konstruktorn för denna klass måste användas efter ändring av sidinställning och cellstil.

```csharp
public class GridSheetRender
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [GridSheetRender](gridsheetrender/)(Worksheet, GridImageOrPrintOptions) | Konstruktionen av SheetRender, behöver kalkylblad och ImageOrPrintOptions som parametrar |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [PageCount](../../aspose.cells.griddesktop.data/gridsheetrender/pagecount/) { get; } | Hämtar det totala sidantalet för aktuellt kalkylblad. |
| [PageScale](../../aspose.cells.griddesktop.data/gridsheetrender/pagescale/) { get; } | Hämtar beräknad sidskala för bladet. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [GetPageSizeInch](../../aspose.cells.griddesktop.data/gridsheetrender/getpagesizeinch/)(int) | Hämta sidstorlek i tum för den genererade bilden. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage)(int) | Rendera en viss sida till ett Bitmap-objekt. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_3)(int, Stream) | Rendera en viss sida till en ström. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_4)(int, string) | Rendera en viss sida till en fil. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_1)(int, Graphics, float, float) | Rendera en viss sida till en Graphics |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_2)(int, Graphics, float, float, float, float) | Rendera en viss sida till en Graphics |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter)(PrinterSettings) | Rendera kalkylblad till Printer |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter_2)(string) | Rendera kalkylblad till Printer |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter_1)(PrinterSettings, string) | Rendera kalkylblad till Printer |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter_3)(string, string) | Rendera kalkylblad till Printer |
| [ToTiff](../../aspose.cells.griddesktop.data/gridsheetrender/totiff/#totiff)(Stream) | Rendera hela kalkylbladet som Tiff Image till en ström. |
| [ToTiff](../../aspose.cells.griddesktop.data/gridsheetrender/totiff/#totiff_1)(string) | Rendera hela kalkylbladet som Tiff Image till en fil. |

### Se även

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


