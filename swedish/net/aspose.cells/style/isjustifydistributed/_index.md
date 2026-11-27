---
title: "Style.IsJustifyDistributed"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style property. Anger om cellerna ska använda justerad eller distribuerad justering på den sista textraden"
type: docs
url: /sv/net/aspose.cells/style/isjustifydistributed/
---
## Style.IsJustifyDistributed property

Anger om cellerna ska ha justerad eller fördelad justering på den sista textraden.

```csharp
public bool IsJustifyDistributed { get; set; }
```

### Anmärkningar

Detta är typiskt för östasiatiska justeringar men inte i andra sammanhang. Fungerar endast när distribuerad horisontell justering används.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsJustifyDistributedDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Åtkomst till cell B3 och ange dess text
            Cell cell = worksheet.Cells["B3"];
            cell.PutValue("Sample Text");

            // Hämta cellens stil och ange IsJustifyDistributed till true
            Style style = cell.GetStyle();
            style.IsJustifyDistributed = true;
            cell.SetStyle(style);

            // Spara arbetsboken
            workbook.Save("output.xlsx");

            // Verifiera egenskapen
            Console.WriteLine("IsJustifyDistributed: " + cell.GetStyle().IsJustifyDistributed);
        }
    }
}
```

### Se även

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


