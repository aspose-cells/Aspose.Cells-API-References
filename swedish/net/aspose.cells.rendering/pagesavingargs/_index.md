---
title: "Klass PageSavingArgs"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Rendering.PageSavingArgs-klass. Information om en sid sparningsprocess"
type: docs
url: /sv/net/aspose.cells.rendering/pagesavingargs/
---
## PageSavingArgs class

Information om en sidlagringsprocess.

```csharp
public class PageSavingArgs
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [PageCount](../../aspose.cells.rendering/pagesavingargs/pagecount/) { get; } | Totalt sidantal. |
| [PageIndex](../../aspose.cells.rendering/pagesavingargs/pageindex/) { get; } | Aktuellt sidindex, nollbaserat. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassPageSavingArgsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med utökad data för flera sidor
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fyll i kalkylbladet för att generera flera sidor vid rendering
            for (int row = 0; row < 150; row++)
            {
                worksheet.Cells[row, 0].Value = $"Row {row + 1} data";
            }

            // Konfigurera PDF‑sparalternativ med sid‑sparningsåteranrop
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.PageSavingCallback = new PageSavingCallback();

            // Spara arbetsbok i PDF-format med paginering
            workbook.Save("RenderingPageSavingDemo.pdf", pdfSaveOptions);
        }

        private class PageSavingCallback : IPageSavingCallback
        {
            public void PageStartSaving(PageStartSavingArgs args)
            {
                Console.WriteLine($"Saving page {args.PageIndex + 1} of {args.PageCount}");
                
                if (args.PageIndex == 0)
                {
                    Console.WriteLine("Processing cover page...");
                }
            }

            public void PageEndSaving(PageEndSavingArgs args)
            {
                // Valfritt: Lägg till eventuell slut‑på‑sida‑behandling här
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


