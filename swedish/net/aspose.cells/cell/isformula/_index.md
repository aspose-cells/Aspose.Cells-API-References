---
title: "Cell.IsFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-egenskap. Anger om den angivna cellen innehåller en formel"
type: docs
url: /sv/net/aspose.cells/cell/isformula/
---
## Cell.IsFormula property

Anger om den angivna cellen innehåller en formel.

```csharp
public bool IsFormula { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsFormulaDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till formel i cell A1
            worksheet.Cells["A1"].Formula = "=1+2";
            
            // Lägg till vanligt värde i cell A2
            worksheet.Cells["A2"].PutValue("Test");
            
            // Kontrollera om celler innehåller formler
            Console.WriteLine("A1 is formula: " + worksheet.Cells["A1"].IsFormula);
            Console.WriteLine("A2 is formula: " + worksheet.Cells["A2"].IsFormula);
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


