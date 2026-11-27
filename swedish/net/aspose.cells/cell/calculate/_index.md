---
title: "Cell.Calculate"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-metod. Beräknar cellens formel"
type: docs
url: /sv/net/aspose.cells/cell/calculate/
---
## Cell.Calculate method

Beräknar cellens formel.

```csharp
public void Calculate(CalculationOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| alternativ | CalculationOptions | Alternativ för beräkning |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodCalculateWithCalculationOptionsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ange en enkel formel i cell A1
            Cell cellA1 = worksheet.Cells["A1"];
            cellA1.Formula = "=SUM(1, 2, 3)";
            
            // Beräkna med standardalternativ
            cellA1.Calculate(new CalculationOptions());
            Console.WriteLine("A1 value after calculation: " + cellA1.Value);

            // Ange en matrisformel i området B1:D1
            Cell cellB1 = worksheet.Cells["B1"];
            cellB1.SetArrayFormula("={1,2,3}", 1, 3);
            
            // Beräkna matrisformeln med alternativ
            cellB1.Calculate(new CalculationOptions());
            Console.WriteLine("B1 value after calculation: " + cellB1.Value);

            // Ange en mer komplex formel i cell A2
            Cell cellA2 = worksheet.Cells["A2"];
            cellA2.Formula = "=IF(A1>5, \"Greater\", \"Less or equal\")";
            
            // Beräkna med alternativ
            cellA2.Calculate(new CalculationOptions());
            Console.WriteLine("A2 value after calculation: " + cellA2.Value);
        }
    }
}
```

### Se även

* class [CalculationOptions](../../calculationoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


