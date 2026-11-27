---
title: "Klass SheetRender"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Rendering.SheetRender-klass. Representerar en kalkylbladsrendering som kan rendera kalkylblad till olika bilder såsom BMP, PNG, JPEG, TIFF.. Konstruktorn för denna klass måste användas efter ändring av sidinställnings‑cellenstil"
type: docs
url: /sv/net/aspose.cells.rendering/sheetrender/
---
## SheetRender class

Representerar en arbetsbladsrendering som kan rendera arbetsblad till olika bilder såsom (BMP, PNG, JPEG, TIFF…). Konstruktorn för denna klass måste användas efter ändring av sidinställning och cellstil.

```csharp
public class SheetRender
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [SheetRender](sheetrender/)(Worksheet, ImageOrPrintOptions) | Konstruktionen av SheetRender, behöver kalkylblad och ImageOrPrintOptions som parametrar |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [PageCount](../../aspose.cells.rendering/sheetrender/pagecount/) { get; } | Hämtar det totala sidantalet för aktuellt kalkylblad. |
| [PageScale](../../aspose.cells.rendering/sheetrender/pagescale/) { get; } | Hämtar beräknad sidskala för bladet. Returnerar den inställda skalan om [`Zoom`](../../aspose.cells/pagesetup/zoom/) är satt. Annars returneras den beräknade skalan enligt [`FitToPagesWide`](../../aspose.cells/pagesetup/fittopageswide/) och [`FitToPagesTall`](../../aspose.cells/pagesetup/fittopagestall/). |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [CustomPrint](../../aspose.cells.rendering/sheetrender/customprint/)(bool, PrintPageEventArgs) | Klienten kan styra sidinställningarna för skrivaren när varje sida skrivs ut med denna funktion. |
| [Dispose](../../aspose.cells.rendering/sheetrender/dispose/)() | Frigör resurser som skapats och används för rendering. |
| [GetPageSizeInch](../../aspose.cells.rendering/sheetrender/getpagesizeinch/)(int) | Hämta sidstorlek i tum för den genererade bilden. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage)(int) | Rendera en viss sida till ett Bitmap-objekt. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_3)(int, Stream) | Rendera en viss sida till en ström. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_4)(int, string) | Rendera en viss sida till en fil. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_1)(int, Graphics, float, float) | Rendera en viss sida till en Graphics |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_2)(int, Graphics, float, float, float, float) | Rendera en viss sida till en Graphics |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter)(PrinterSettings) | Rendera kalkylblad till Printer |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_2)(string) | Rendera kalkylblad till Printer |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_1)(PrinterSettings, string) | Rendera kalkylblad till Printer |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_4)(string, string) | Rendera kalkylblad till Printer |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_3)(string, int, int) | (**Obsolete.**) Rendera kalkylblad till Printer |
| [ToTiff](../../aspose.cells.rendering/sheetrender/totiff/#totiff)(Stream) | Rendera hela kalkylbladet som Tiff Image till en ström. |
| [ToTiff](../../aspose.cells.rendering/sheetrender/totiff/#totiff_1)(string) | Rendera hela kalkylbladet som Tiff Image till en fil. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassSheetRenderDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Lägg till exempeldata
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Konfigurera sidinställning
            PageSetup pageSetup = sheet.PageSetup;
            pageSetup.PrintArea = "1:10";
            pageSetup.SetFitToPages(1, 1);

            // Skapa SheetRender och demonstrera kärnfunktionalitet
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            SheetRender sr = new SheetRender(sheet, options);
            
            Console.WriteLine($"Number of pages: {sr.PageCount}");
            Console.WriteLine($"Page scale: {sr.PageScale * 100}%");
            
            // Rendera första sidan till bild (demonstration)
            sr.ToImage(0, "output_page1.png");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


