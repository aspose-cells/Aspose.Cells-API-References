---
title: "Cell.FloatValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-egenskap. Hämtar flyttalsvärdet som finns i cellen"
type: docs
url: /sv/net/aspose.cells/cell/floatvalue/
---
## Cell.FloatValue property

Hämtar flyttalsvärdet som finns i cellen.

```csharp
public float FloatValue { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyFloatValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange numeriskt värde direkt
            worksheet.Cells["A1"].PutValue(3.14f);
            Console.WriteLine("FloatValue of A1: " + worksheet.Cells["A1"].FloatValue);
            
            // Ange formel som returnerar flyttal
            worksheet.Cells["A2"].Formula = "=3.5*2";
            workbook.CalculateFormula();
            Console.WriteLine("FloatValue of A2: " + worksheet.Cells["A2"].FloatValue);
            
            // Demonstrera FloatValue med delad formel
            worksheet.Cells["B1"].Formula = "=5-2";
            workbook.CalculateFormula();
            worksheet.Cells["B1"].SetSharedFormula("=5-2", 3, 1);
            workbook.CalculateFormula();
            Console.WriteLine("FloatValue of B3: " + worksheet.Cells["B3"].FloatValue);
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


