---
title: "WorkbookRender.PageCount"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookRender-egenskap. Hämtar det totala sidantalet för arbetsboken"
type: docs
url: /sv/net/aspose.cells.rendering/workbookrender/pagecount/
---
## WorkbookRender.PageCount property

Hämtar det totala sidantalet för arbetsboken.

```csharp
public int PageCount { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookRenderPropertyPageCountDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Page 1 Content");
            
            // Lägg till ett andra kalkylblad
            workbook.Worksheets.Add();
            worksheet = workbook.Worksheets[1];
            worksheet.Cells["A1"].PutValue("Page 2 Content");

            // Skapa renderingsalternativ och arbetsboksgenererare
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                OnePagePerSheet = true
            };
            
            WorkbookRender renderer = new WorkbookRender(workbook, options);

            // Demonstrera användning av PageCount
            Console.WriteLine($"Total pages to render: {renderer.PageCount}");
            
            // Rendera varje sida till bild
            for (int i = 0; i < renderer.PageCount; i++)
            {
                string outputPath = $"Page_{i}.png";
                renderer.ToImage(i, outputPath);
                Console.WriteLine($"Rendered page {i+1} to {outputPath}");
            }
        }
    }
}
```

### Se även

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


