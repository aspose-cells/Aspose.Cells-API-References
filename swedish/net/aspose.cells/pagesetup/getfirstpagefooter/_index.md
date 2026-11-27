---
title: "PageSetup.GetFirstPageFooter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-metod. Hämtar ett skript som formaterar första sidfoten i en Excel-fil"
type: docs
url: /sv/net/aspose.cells/pagesetup/getfirstpagefooter/
---
## PageSetup.GetFirstPageFooter method

Hämtar ett skript som formaterar första sidfot på en Excel-fil.

```csharp
public string GetFirstPageFooter(int section)
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
    public class PageSetupMethodGetFirstPageFooterWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ställ in första sidfoten
            worksheet.PageSetup.SetFirstPageFooter(1, "First Page Footer");

            // Hämta och skriv ut första sidfoten
            string footer = worksheet.PageSetup.GetFirstPageFooter(1);
            Console.WriteLine("First Page Footer: " + footer);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


