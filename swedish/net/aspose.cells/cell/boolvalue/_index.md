---
title: "Cell.BoolValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-egenskap. Hämtar det booleska värdet som finns i cellen"
type: docs
url: /sv/net/aspose.cells/cell/boolvalue/
---
## Cell.BoolValue property

Hämtar det booleska värdet som finns i cellen.

```csharp
public bool BoolValue { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyBoolValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Cell cell = cells[0, 0];
            
            // Ställ in en formel som utvärderas till ett booleskt värde
            cell.Formula = "=2.01>2";
            
            // Beräkna formeln för att få resultatet
            workbook.CalculateFormula();
            
            // Demonstrera BoolValue-egenskapen
            Console.WriteLine("Cell BoolValue: " + cell.BoolValue);
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


