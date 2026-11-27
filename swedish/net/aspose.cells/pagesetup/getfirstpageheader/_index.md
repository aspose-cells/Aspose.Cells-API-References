---
title: "PageSetup.GetFirstPageHeader"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-metod. Hämtar ett skript som formaterar första sidhuvudet i en Excel-fil."
type: docs
url: /sv/net/aspose.cells/pagesetup/getfirstpageheader/
---
## PageSetup.GetFirstPageHeader method

Hämtar ett skript som formaterar första sidhuvud på en Excel-fil.

```csharp
public string GetFirstPageHeader(int section)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sektion | Int32 | 0: Vänster sektion, 1: Centrerad sektion, 2: Höger sektion. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodGetFirstPageHeaderWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Kom åt PageSetup.
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Aktivera olika första sidhuvud/sidfot.
            pageSetup.IsHFDiffFirst = true;
            
            // Ställ in sektioner för första sidhuvudet.
            pageSetup.SetFirstPageHeader(0, "&LFirst Page Left Header");
            pageSetup.SetFirstPageHeader(1, "&CFirst Page Center Header");
            pageSetup.SetFirstPageHeader(2, "&RFirst Page Right Header");
            
            // Hämta och visa första sidans rubriksektioner
            Console.WriteLine("First Page Header Sections:");
            Console.WriteLine("Left: " + pageSetup.GetFirstPageHeader(0));
            Console.WriteLine("Center: " + pageSetup.GetFirstPageHeader(1));
            Console.WriteLine("Right: " + pageSetup.GetFirstPageHeader(2));
            
            // Spara arbetsboken
            workbook.Save("PageSetupFirstPageHeaderDemo.xlsx");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


