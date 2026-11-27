---
title: "Cell.Formula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-egenskap. Hämtar eller anger en formel för cellen"
type: docs
url: /sv/net/aspose.cells/cell/formula/
---
## Cell.Formula property

Hämtar eller anger en formel för [`Cell`](../).

```csharp
public string Formula { get; set; }
```

### Anmärkningar

En formelsträng börjar alltid med ett lika-tecken (=). Och vänligen använd alltid komma (,) som parameteravgränsare, till exempel "=SUM(A1, E1, H2)".

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyFormulaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange värden i celler som kommer att användas i formeln
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);
            worksheet.Cells["E1"].PutValue(5);
            worksheet.Cells["A1"].PutValue(100);

            // Ange formel i cell B6
            worksheet.Cells["B6"].Formula = "=SUM(B2:B5, E1) + A1";

            // Beräkna formeln
            workbook.CalculateFormula();

            // Visa resultatet
            Console.WriteLine("Formula result in B6: " + worksheet.Cells["B6"].Value);
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


