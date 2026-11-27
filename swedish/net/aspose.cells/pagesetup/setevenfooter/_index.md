---
title: "PageSetup.SetEvenFooter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup metod. Ställer in ett skript som formaterar den jämna sidfoten i en Excel-fil. Påverkar endast i Excel 2007 när IsHFDiffOddEven är sant"
type: docs
url: /sv/net/aspose.cells/pagesetup/setevenfooter/
---
## PageSetup.SetEvenFooter method

Ställer in ett skript som formaterar den jämna sidfoten i en Excel-fil. Endast effekt i Excel 2007 när IsHFDiffOddEven är sant.

```csharp
public void SetEvenFooter(int section, string footerScript)
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
    public class PageSetupMethodSetEvenFooterWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Aktivera olika header/footer för första och jämna sidor
            pageSetup.IsHFDiffFirst = true;
            pageSetup.IsHFDiffOddEven = true;

            // Ställ in olika sidfottyper
            pageSetup.SetEvenFooter(0, "Even Page Footer");
            pageSetup.SetFooter(0, "Odd Page Footer");
            pageSetup.SetFirstPageFooter(0, "First Page Footer");

            // Spara arbetsboken
            workbook.Save("PageSetup_SetEvenFooter_Example.xlsx");

            Console.WriteLine("Workbook saved with even page footer set successfully.");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


