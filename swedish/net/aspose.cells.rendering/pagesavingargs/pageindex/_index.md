---
title: "PageSavingArgs.PageIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSavingArgs-egenskap. Aktuellt sidindex, nollbaserat"
type: docs
url: /sv/net/aspose.cells.rendering/pagesavingargs/pageindex/
---
## PageSavingArgs.PageIndex property

Aktuellt sidindex, nollbaserat.

```csharp
public int PageIndex { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PageSavingArgsPropertyPageIndexDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till lite data i kalkylbladet
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data row {i + 1}";
            }

            // Skapa PDF-sparalternativ
            PdfSaveOptions options = new PdfSaveOptions();
            
            // Ställ in återanropet för sidsparning
            options.PageSavingCallback = new PageSavingCallback();

            // Spara arbetsboken till PDF – detta kommer att utlösa återanropet för varje sida
            workbook.Save("output.pdf", options);
        }
    }

    public class PageSavingCallback : IPageSavingCallback
    {
        public void PageStartSaving(PageStartSavingArgs args)
        {
            // Demonstrera användning av PageIndex-egenskapen
            Console.WriteLine($"Starting to save page {args.PageIndex + 1}");
        }

        public void PageEndSaving(PageEndSavingArgs args)
        {
            // Används inte i detta exempel
        }
    }
}
```

### Se även

* class [PageSavingArgs](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


