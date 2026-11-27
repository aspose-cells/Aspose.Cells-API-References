---
title: "PageSetup.SetFirstPageFooter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-metod. Ställer in ett skript som formaterar den första sidfoten i en Excel-fil"
type: docs
url: /sv/net/aspose.cells/pagesetup/setfirstpagefooter/
---
## PageSetup.SetFirstPageFooter method

Ställer in ett skript som formaterar den första sidfoten i en Excel-fil.

```csharp
public void SetFirstPageFooter(int section, string footerScript)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sektion | Int32 | 0: Vänster sektion, 1: Centrerad sektion, 2: Höger sektion. |
| footerScript | String | Sidfotformatskript. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetFirstPageFooterWithInt32StringDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hämta PageSetup-objektet
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Ställ in olika sidhuvuden/sidfötter för första sidan
            pageSetup.IsHFDiffFirst = true;
            
            // Ställ in första sidfot med sektionsindex och text
            pageSetup.SetFirstPageFooter(0, "First Page Footer Text");
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
            
            Console.WriteLine("First page footer set successfully.");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


