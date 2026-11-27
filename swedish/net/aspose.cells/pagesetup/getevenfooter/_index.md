---
title: "PageSetup.GetEvenFooter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-metod. Hämtar ett skript som formaterar den jämna sidfoten i en Excel-fil"
type: docs
url: /sv/net/aspose.cells/pagesetup/getevenfooter/
---
## PageSetup.GetEvenFooter method

Hämtar ett skript som formaterar jämn sidfot i en Excel-fil.

```csharp
public string GetEvenFooter(int section)
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
    public class PageSetupMethodGetEvenFooterWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Aktivera olika sidhuvuden/sidfötter för udda och jämna sidor
            pageSetup.IsHFDiffOddEven = true;
            
            // Ställ in jämn sidfot
            pageSetup.SetEvenFooter(0, "Even Page Footer");
            
            // Hämta och visa den jämna sidfoten
            string evenFooter = pageSetup.GetEvenFooter(0);
            Console.WriteLine("Even Footer: " + evenFooter);
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


