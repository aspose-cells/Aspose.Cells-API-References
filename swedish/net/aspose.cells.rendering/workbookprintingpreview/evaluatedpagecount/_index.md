---
title: "WorkbookPrintingPreview.EvaluatedPageCount"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookPrintingPreview-egenskap. Utvärdera det totala sidantalet för denna arbetsbok"
type: docs
url: /sv/net/aspose.cells.rendering/workbookprintingpreview/evaluatedpagecount/
---
## WorkbookPrintingPreview.EvaluatedPageCount property

Utvärdera det totala sidantalet i den här arbetsboken

```csharp
public int EvaluatedPageCount { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookPrintingPreviewPropertyEvaluatedPageCountDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i kalkylbladet
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[i, 0].PutValue("Row " + (i + 1));
            }

            // Skapa alternativ för utskriftsförhandsgranskning
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // Skapa utskriftsförhandsgranskning för arbetsbok
            WorkbookPrintingPreview printingPreview = new WorkbookPrintingPreview(workbook, options);
            
            // Hämta och visa det utvärderade sidantalet
            Console.WriteLine("Evaluated Page Count: " + printingPreview.EvaluatedPageCount);
        }
    }
}
```

### Se även

* class [WorkbookPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


