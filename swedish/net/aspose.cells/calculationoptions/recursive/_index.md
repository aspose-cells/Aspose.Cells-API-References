---
title: "CalculationOptions.Recursive"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CalculationOptions-egenskap. Anger om de beroende cellerna ska beräknas rekursivt när en cell beräknas och den beror på andra celler. Standardvärdet är true"
type: docs
url: /sv/net/aspose.cells/calculationoptions/recursive/
---
## CalculationOptions.Recursive property

Anger om beroende celler ska beräknas rekursivt när en cell beräknas och den beror på andra celler. Standardvärdet är true.

```csharp
public bool Recursive { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyRecursiveDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Skapa cirkulär referens
            cells["A1"].Formula = "=A2";
            cells["A2"].Formula = "=A1";

            // Första beräkning med Recursive=true (standard)
            CalculationOptions copts = new CalculationOptions();
            copts.Recursive = true;
            wb.CalculateFormula(copts);
            Console.WriteLine("Recursive calculation result (A2): " + cells["A2"].Value);

            // Andra beräkning med Recursive=false
            copts.Recursive = false;
            wb.CalculateFormula(copts);
            Console.WriteLine("Non-recursive calculation result (A2): " + cells["A2"].Value);
        }
    }
}
```

### Se även

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


