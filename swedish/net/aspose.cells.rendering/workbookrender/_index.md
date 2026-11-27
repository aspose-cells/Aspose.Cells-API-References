---
title: "Klass WorkbookRender"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Rendering.WorkbookRender-klass. Representerar en arbetsboksrendering. Konstruktorn för denna klass måste användas efter ändring av sidinställningens cellstil"
type: docs
url: /sv/net/aspose.cells.rendering/workbookrender/
---
## WorkbookRender class

Representerar en arbetsboksrendering. Konstruktorn för denna klass måste användas efter ändring av pagesetup och cell style.

```csharp
public class WorkbookRender
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [WorkbookRender](workbookrender/)(Workbook, ImageOrPrintOptions) | Konstruktionen av WorkbookRender |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [PageCount](../../aspose.cells.rendering/workbookrender/pagecount/) { get; } | Hämtar det totala sidantalet för arbetsboken. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [CustomPrint](../../aspose.cells.rendering/workbookrender/customprint/)(bool, PrintPageEventArgs) | Klienten kan styra sidinställningarna för skrivaren när varje sida skrivs ut med denna funktion. |
| [Dispose](../../aspose.cells.rendering/workbookrender/dispose/)() | Frigör resurser som skapats och används för rendering. |
| [GetPageSizeInch](../../aspose.cells.rendering/workbookrender/getpagesizeinch/)(int) | Hämta sidstorlek i tum för den genererade bilden. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage)(int) | Rendera en viss sida till ett Bitmap-objekt. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_3)(Stream) | Rendera hela arbetsboken som Tiff-bild till en ström. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_4)(string) | Rendera hela arbetsboken som Tiff-bild till en fil. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_1)(int, Stream) | Rendera en viss sida till en ström. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_2)(int, string) | Rendera en viss sida till en fil. |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter)(PrinterSettings) | Rendera arbetsboken till skrivare |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_2)(string) | Rendera arbetsboken till skrivare |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_1)(PrinterSettings, string) | Rendera arbetsboken till skrivare |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_4)(string, string) | Rendera arbetsboken till skrivare |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_3)(string, int, int) | (**Obsolete.**) Rendera arbetsboken till skrivare |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassWorkbookRenderDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata och ange sidstorlek
            worksheet.Cells["A1"].PutValue("Workbook Render Demo");
            worksheet.PageSetup.PaperSize = PaperSizeType.PaperLetter;

            // Skapa bildalternativ
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // Skapa arbetsboksrendering och hämta sidstorlek
            WorkbookRender render = new WorkbookRender(workbook, options);
            float[] pageSize = render.GetPageSizeInch(0);
            
            // Skriv ut resultaten
            Console.WriteLine($"Page Width: {pageSize[0]} inches");
            Console.WriteLine($"Page Height: {pageSize[1]} inches");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


