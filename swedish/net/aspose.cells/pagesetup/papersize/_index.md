---
title: "PageSetup.PaperSize"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-egenskap. Representerar papperets storlek"
type: docs
url: /sv/net/aspose.cells/pagesetup/papersize/
---
## PageSetup.PaperSize property

Representerar papperets storlek.

```csharp
public PaperSizeType PaperSize { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPaperSizeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ställ in papperstorleken till kuvert B6
            sheet.PageSetup.PaperSize = PaperSizeType.PaperEnvelopeB6;

            // Skriv ut den aktuella papperstorleken
            Console.WriteLine("Current paper size: " + sheet.PageSetup.PaperSize);

            // Spara arbetsboken
            workbook.Save("PageSetup_PaperSizeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [PaperSizeType](../../papersizetype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


