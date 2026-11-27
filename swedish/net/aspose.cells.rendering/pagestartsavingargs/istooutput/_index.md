---
title: "PageStartSavingArgs.IsToOutput"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageStartSavingArgs‑egenskap. Hämtar eller anger ett värde som visar om sidan ska skrivas ut. Standardvärdet är true"
type: docs
url: /sv/net/aspose.cells.rendering/pagestartsavingargs/istooutput/
---
## PageStartSavingArgs.IsToOutput property

Hämtar eller anger ett värde som indikerar om sidan ska skrivas ut. Standardvärdet är true.

```csharp
public bool IsToOutput { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PageStartSavingArgsPropertyIsToOutputDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i data för att skapa flera sidor
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[i, 0].Value = "Data Row " + (i + 1);
                // Korrigerat: Åtkomst till radhöjd via kalkylbladets Rows‑samling
                worksheet.Cells.Rows[i].Height = 50;
            }

            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.PageSavingCallback = new CustomPageSavingCallback();

            workbook.Save("PageOutputDemo.pdf", saveOptions);
        }

        private class CustomPageSavingCallback : IPageSavingCallback
        {
            public void PageStartSaving(PageStartSavingArgs args)
            {
                // Läs aktuellt värde
                Console.WriteLine($"Page {args.PageIndex + 1} - Initial IsToOutput: {args.IsToOutput}");

                // Hoppa över varje jämnt numrerad sida (1‑baserad numrering)
                if ((args.PageIndex + 1) % 2 == 0)
                {
                    args.IsToOutput = false;
                    Console.WriteLine($"Disabling output for page {args.PageIndex + 1}");
                }
            }

            public void PageEndSaving(PageEndSavingArgs args)
            {
                // Implementering krävs inte för denna demonstration
            }
        }
    }
}
```

### Se även

* class [PageStartSavingArgs](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


