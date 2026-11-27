---
title: "Cell.IsDynamicArrayFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-egenskap. Anger om cellens formel är en dynamisk arrayformel (true) eller en äldre arrayformel (false)"
type: docs
url: /sv/net/aspose.cells/cell/isdynamicarrayformula/
---
## Cell.IsDynamicArrayFormula property

Anger om cellens formel är en dynamisk matrisformel (true) eller en äldre matrisformel (false).

```csharp
public bool IsDynamicArrayFormula { get; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsDynamicArrayFormulaDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ställ in en dynamisk arrayformel i cell A1
            worksheet.Cells["A1"].SetDynamicArrayFormula("=B1:B3", new FormulaParseOptions(), false);
            
            // Kontrollera om cellen innehåller en dynamisk arrayformel
            Console.WriteLine("Is A1 a dynamic array formula? " + worksheet.Cells["A1"].IsDynamicArrayFormula);

            // Spara arbetsboken
            string outputPath = "DynamicArrayFormulaDemo.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);

            Console.WriteLine("Workbook saved with dynamic array formula at: " + outputPath);
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


