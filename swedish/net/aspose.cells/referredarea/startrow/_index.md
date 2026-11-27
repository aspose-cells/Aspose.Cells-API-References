---
title: "ReferredArea.StartRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ReferredArea-egenskapen. Startraden för området"
type: docs
url: /sv/net/aspose.cells/referredarea/startrow/
---
## ReferredArea.StartRow property

Startraden för området.

```csharp
public int StartRow { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaPropertyStartRowDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok och ett kalkylblad
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i lite exempeldata
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);

            // Skapa ett namngivet område som refererar till A2:A4
            int index = workbook.Worksheets.Names.Add("MyRange");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet1!$A$2:$A$4";

            // Hämta det refererade området med omräkningsparameter
            ReferredArea area = name.GetReferredAreas(false)[0];

            // Demonstrera StartRow-egenskapen
            Console.WriteLine("Start Row: " + area.StartRow); // Should output 1 (0-based)
            Console.WriteLine("End Row: " + area.EndRow);     // Should output 3 (0-based)
            Console.WriteLine("Row Count: " + (area.EndRow - area.StartRow + 1)); // Should output 3

            // Iterera genom det refererade området med StartRow och EndRow
            for (int row = area.StartRow; row <= area.EndRow; row++)
            {
                Cell cell = worksheet.Cells[row, 0]; // Column 0 is A
                Console.WriteLine("Value at row " + row + ": " + cell.Value);
            }
        }
    }
}
```

### Se även

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


