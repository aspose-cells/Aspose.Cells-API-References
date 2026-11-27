---
title: "WorkbookPrintingPreview.WorkbookPrintingPreview"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookPrintingPreview-konstruktor. Konstruktionen av WorkbookPrintingPreview"
type: docs
url: /sv/net/aspose.cells.rendering/workbookprintingpreview/workbookprintingpreview/
---
## WorkbookPrintingPreview constructor

Konstruktionen av WorkbookPrintingPreview

```csharp
public WorkbookPrintingPreview(Workbook workbook, ImageOrPrintOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arbetsbok | Arbetsbok | Ange vilken arbetsbok som ska skrivas ut. |
| alternativ | ImageOrPrintOptions | ImageOrPrintOptions innehåller vissa egenskaper för utdata |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookPrintingPreviewMethodCtorWithWorkbookImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Printing Preview");
            
            // Ställ in utskriftsalternativ
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PrintingPage = PrintingPageType.Default;

            // Skapa utskriftsförhandsgranskning med arbetsbok och alternativ
            WorkbookPrintingPreview preview = new WorkbookPrintingPreview(workbook, options);
            
            // Visa sidantal
            Console.WriteLine("Total pages: " + preview.EvaluatedPageCount);
        }
    }
}
```

### Se även

* class [Workbook](../../../aspose.cells/workbook/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [WorkbookPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


