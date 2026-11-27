---
title: "ImageOrPrintOptions.PageIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions‑egenskap. Hämtar eller anger det nollbaserade indexet för den första sidan som ska sparas"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/pageindex/
---
## ImageOrPrintOptions.PageIndex property

Hämtar eller anger det 0‑baserade indexet för den första sidan som ska sparas.

```csharp
public int PageIndex { get; set; }
```

### Anmärkningar

Standard är 0.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyPageIndexDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata på flera sidor
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Data Row " + (i + 1);
            }

            // Ställ in bild-/utskriftsalternativ
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PageIndex = 1; // Start from second page (0-based index would be 1)
            options.PageCount = 1; // Only process one page

            // Skapa sheet render för det första kalkylbladet
            SheetRender render = new SheetRender(worksheet, options);

            // Spara till PDF med rätt API‑metod
            render.ToImage(0, "output.pdf");
            Console.WriteLine("Saved page 2 to PDF successfully.");
        }
    }
}
```

### Se även

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


