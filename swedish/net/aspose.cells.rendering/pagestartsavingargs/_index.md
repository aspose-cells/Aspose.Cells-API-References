---
title: "Class PageStartSavingArgs"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Rendering.PageStartSavingArgs-klass. Information för en sida när sparningsprocessen startar"
type: docs
url: /sv/net/aspose.cells.rendering/pagestartsavingargs/
---
## PageStartSavingArgs class

Information om att en sida påbörjar lagringsprocessen.

```csharp
public class PageStartSavingArgs : PageSavingArgs
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [IsToOutput](../../aspose.cells.rendering/pagestartsavingargs/istooutput/) { get; set; } | Hämtar eller anger ett värde som indikerar om sidan ska skrivas ut. Standardvärdet är true. |
| [PageCount](../../aspose.cells.rendering/pagesavingargs/pagecount/) { get; } | Totalt sidantal.(ärvt från [`PageSavingArgs`](../pagesavingargs/).) |
| [PageIndex](../../aspose.cells.rendering/pagesavingargs/pageindex/) { get; } | Aktuellt sidindex, nollbaserat.(ärvt från [`PageSavingArgs`](../pagesavingargs/).) |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassPageStartSavingArgsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till lite exempeldata
            worksheet.Cells["A1"].PutValue("Hello World");
            
            PdfSaveOptions options = new PdfSaveOptions();
            options.PageSavingCallback = new CustomPageSavingCallback();
            
            workbook.Save("output.pdf", options);
        }
    }
    
    public class CustomPageSavingCallback : IPageSavingCallback
    {
        public void PageStartSaving(PageStartSavingArgs args)
        {
            Console.WriteLine($"Starting to save page {args.PageIndex}");
        }
        
        public void PageEndSaving(PageEndSavingArgs args)
        {
            // Valfri implementation
        }
    }
}
```

### Se även

* class [PageSavingArgs](../pagesavingargs/)
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


