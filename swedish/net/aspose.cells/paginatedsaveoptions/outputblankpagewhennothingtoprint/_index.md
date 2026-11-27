---
title: "PaginatedSaveOptions.OutputBlankPageWhenNothingToPrint"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PaginatedSaveOptions-egenskap. Anger om en tom sida ska skrivas ut när det inte finns något att skriva ut"
type: docs
url: /sv/net/aspose.cells/paginatedsaveoptions/outputblankpagewhennothingtoprint/
---
## PaginatedSaveOptions.OutputBlankPageWhenNothingToPrint property

Anger om en tom sida ska skrivas ut när det inte finns något att skriva ut.

```csharp
public bool OutputBlankPageWhenNothingToPrint { get; set; }
```

### Anmärkningar

Standard är true.

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyOutputBlankPageWhenNothingToPrintDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett kalkylblad och dölj det (simulerar att det inte finns något att skriva ut)
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.IsVisible = false;

            // Ange PDF‑sparalternativ med OutputBlankPageWhenNothingToPrint = false
            PdfSaveOptions options = new PdfSaveOptions
            {
                OutputBlankPageWhenNothingToPrint = false
            };

            // Spara till PDF – ingen tom sida bör genereras
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "OutputNoBlankPage.pdf");
            workbook.Save(outputPath, options);

            // Ändra alternativet till true
            options.OutputBlankPageWhenNothingToPrint = true;

            // Spara igen – en tom sida bör genereras
            outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "OutputWithBlankPage.pdf");
            workbook.Save(outputPath, options);
        }
    }
}
```

### Se även

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


