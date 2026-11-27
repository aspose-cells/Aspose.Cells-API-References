---
title: "PageSetup.Order"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-egenskap. Representerar den ordning som Microsoft Excel använder för att numrera sidor när en stor arbetsbok skrivs ut"
type: docs
url: /sv/net/aspose.cells/pagesetup/order/
---
## PageSetup.Order property

Representerar den ordning som Microsoft Excel använder för att numrera sidor när ett stort arbetsblad skrivs ut.

```csharp
public PrintOrderType Order { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyOrderDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ställ in utskriftsordning till DownThenOver
            sheet.PageSetup.Order = PrintOrderType.DownThenOver;
            Console.WriteLine("Print order set to: " + sheet.PageSetup.Order);

            // Spara arbetsboken i olika format
            workbook.Save("output_DownThenOver.xlsx", SaveFormat.Xlsx);
            workbook.Save("output_DownThenOver.xls", SaveFormat.Excel97To2003);

            // Ändra utskriftsordningen till OverThenDown
            sheet.PageSetup.Order = PrintOrderType.OverThenDown;
            Console.WriteLine("Print order changed to: " + sheet.PageSetup.Order);

            // Spara igen med olika format
            workbook.Save("output_OverThenDown.xlsx", SaveFormat.Xlsx);
            workbook.Save("output_OverThenDown.xls", SaveFormat.Excel97To2003);
        }
    }
}
```

### Se även

* enum [PrintOrderType](../../printordertype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


