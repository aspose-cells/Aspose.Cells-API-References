---
title: "PageSetup.GetFooter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup‑metod. Hämtar ett skript som formaterar sidfoten i en Excel‑fil"
type: docs
url: /sv/net/aspose.cells/pagesetup/getfooter/
---
## PageSetup.GetFooter method

Hämtar ett skript som formaterar sidfot i en Excel-fil.

```csharp
public string GetFooter(int section)
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
    public class PageSetupMethodGetFooterWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ställ in olika sidfotsektioner
            worksheet.PageSetup.SetFooter(1, "odd");
            worksheet.PageSetup.SetFirstPageFooter(1, "first");
            worksheet.PageSetup.SetEvenFooter(1, "even");

            // Hämta och visa sidfotsektionerna
            Console.WriteLine("First Page Footer: " + worksheet.PageSetup.GetFirstPageFooter(1));
            Console.WriteLine("Even Page Footer: " + worksheet.PageSetup.GetEvenFooter(1));
            Console.WriteLine("Odd Page Footer: " + worksheet.PageSetup.GetFooter(1));
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


