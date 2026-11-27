---
title: "PageEndSavingArgs.HasMorePages"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageEndSavingArgs‑egenskap. Hämtar eller anger ett värde som visar om fler sidor ska skrivas ut. Standardvärdet är true"
type: docs
url: /sv/net/aspose.cells.rendering/pageendsavingargs/hasmorepages/
---
## PageEndSavingArgs.HasMorePages property

Hämtar eller anger ett värde som indikerar om fler sidor ska skrivas ut. Standardvärdet är true.

```csharp
public bool HasMorePages { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PageEndSavingArgsPropertyHasMorePagesDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med data som sträcker sig över flera sidor
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 500; i++)
            {
                worksheet.Cells[i, 0].Value = $"Row {i + 1}";
            }

            // Skapa PDF‑sparalternativ med anpassad sidhantering
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.PageSavingCallback = new PageControlCallback();

            // Spara arbetsboken med sidbegränsning
            workbook.Save("PropertyHasMorePagesDemo.pdf", saveOptions);
        }
    }

    internal class PageControlCallback : IPageSavingCallback
    {
        private int pageCount = 0;

        public void PageStartSaving(PageStartSavingArgs args)
        {
            // Används inte i denna demonstration
        }

        public void PageEndSaving(PageEndSavingArgs args)
        {
            // Läs aktuellt egenskapsvärde
            Console.WriteLine($"Page {pageCount} - Initial HasMorePages: {args.HasMorePages}");

            // Ändra egenskap efter första sidan
            if (pageCount == 0)
            {
                args.HasMorePages = false;
                Console.WriteLine($"Page {pageCount} - Updated HasMorePages: {args.HasMorePages}");
            }

            pageCount++;
        }
    }
}
```

### Se även

* class [PageEndSavingArgs](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


