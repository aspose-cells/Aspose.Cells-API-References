---
title: "Class PageEndSavingArgs"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Rendering.PageEndSavingArgs-klass. Information för en sida när sparningsprocessen avslutas"
type: docs
url: /sv/net/aspose.cells.rendering/pageendsavingargs/
---
## PageEndSavingArgs class

Information för en sida avslutar sparprocessen.

```csharp
public class PageEndSavingArgs : PageSavingArgs
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [HasMorePages](../../aspose.cells.rendering/pageendsavingargs/hasmorepages/) { get; set; } | Hämtar eller anger ett värde som indikerar om fler sidor ska skrivas ut. Standardvärdet är true. |
| [PageCount](../../aspose.cells.rendering/pagesavingargs/pagecount/) { get; } | Totalt sidantal.(ärvt från [`PageSavingArgs`](../pagesavingargs/).) |
| [PageIndex](../../aspose.cells.rendering/pagesavingargs/pageindex/) { get; } | Aktuellt sidindex, nollbaserat.(ärvt från [`PageSavingArgs`](../pagesavingargs/).) |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassPageEndSavingArgsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data i kalkylbladet
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Skapa en instans av PdfSaveOptions
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Ställ in PageEndSaving‑callbacken
            saveOptions.PageSavingCallback = new PageEndSavingArgsTest();

            // Spara arbetsboken med callbacken
            workbook.Save("output.pdf", saveOptions);
        }
    }

    public class PageEndSavingArgsTest : IPageSavingCallback
    {
        public void PageEndSaving(PageEndSavingArgs args)
        {
            Console.WriteLine($"Finished saving page {args.PageIndex}");
        }

        public void PageStartSaving(PageStartSavingArgs args)
        {
            // Implementering behövs inte för den här demonstrationen
        }
    }
}
```

### Se även

* class [PageSavingArgs](../pagesavingargs/)
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


