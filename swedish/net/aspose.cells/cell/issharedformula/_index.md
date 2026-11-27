---
title: "Cell.IsSharedFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell egenskap. Anger om cellens formel är en del av en delad formel"
type: docs
url: /sv/net/aspose.cells/cell/issharedformula/
---
## Cell.IsSharedFormula property

Anger om cellens formel är en del av en delad formel.

```csharp
public bool IsSharedFormula { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsSharedFormulaDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ange delad formel i ett område
            worksheet.Cells["B2"].Formula = "=A2*2";
            worksheet.Cells["B2"].Copy(worksheet.Cells["B3:B5"]);

            // Kontrollera om celler innehåller delad formel
            Cell cellB2 = worksheet.Cells["B2"];
            Cell cellB3 = worksheet.Cells["B3"];

            Console.WriteLine("Cell B2 IsSharedFormula: " + cellB2.IsSharedFormula);
            Console.WriteLine("Cell B3 IsSharedFormula: " + cellB3.IsSharedFormula);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


