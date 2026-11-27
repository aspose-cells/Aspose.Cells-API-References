---
title: "Cell.IsArrayFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell‑egenskap. Anger om cellens formel är en matrisformel"
type: docs
url: /sv/net/aspose.cells/cell/isarrayformula/
---
## Cell.IsArrayFormula property

Anger om cellens formel är en matrisformel.

```csharp
public bool IsArrayFormula { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsArrayFormulaDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa en matrisformel i cell B2
            worksheet.Cells["B2"].SetArrayFormula("SUM(A1:A10*B1:B10)", 1, 1);
            
            // Kontrollera om cellen innehåller en matrisformel
            bool isArrayFormula = worksheet.Cells["B2"].IsArrayFormula;
            
            // Skriv ut resultatet
            Console.WriteLine("Cell B2 is an array formula: " + isArrayFormula);
            
            // Spara arbetsboken
            workbook.Save("IsArrayFormulaDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


