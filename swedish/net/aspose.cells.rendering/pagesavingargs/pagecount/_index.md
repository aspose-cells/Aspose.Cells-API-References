---
title: "PageSavingArgs.PageCount"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSavingArgs-egenskap. Totalt sidantal"
type: docs
url: /sv/net/aspose.cells.rendering/pagesavingargs/pagecount/
---
## PageSavingArgs.PageCount property

Totalt sidantal.

```csharp
public int PageCount { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PageSavingArgsPropertyPageCountDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och lägg till testdata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till tät innehåll för att skapa flera sidor
            for (int i = 0; i < 500; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }

            // Ställ in sidinställning för att kontrollera paginering
            worksheet.PageSetup.PrintArea = "A1:A50";
            worksheet.PageSetup.PaperSize = PaperSizeType.PaperLetter;

            // Skapa PDF-sparalternativ med återanrop för sidsparning
            PdfSaveOptions options = new PdfSaveOptions();
            options.PageSavingCallback = new PageSavingCallback();

            // Spara till PDF för att utlösa paginering
            workbook.Save("PageSavingDemo.pdf", options);
        }

        private class PageSavingCallback : IPageSavingCallback
        {
            public void PageStartSaving(PageStartSavingArgs args)
            {
                // Kom åt PageCount från händelseargumenten
                Console.WriteLine($"Saving page {args.PageIndex + 1} of {args.PageCount}");
            }

            public void PageEndSaving(PageEndSavingArgs args)
            {
                // Ingen implementation behövs
            }
        }
    }
}
```

### Se även

* class [PageSavingArgs](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


