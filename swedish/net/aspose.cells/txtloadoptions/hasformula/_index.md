---
title: "TxtLoadOptions.HasFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TxtLoadOptions-egenskap. Anger om texten är en formel om den börjar med"
type: docs
url: /sv/net/aspose.cells/txtloadoptions/hasformula/
---
## TxtLoadOptions.HasFormula property

Anger om texten är en formel om den börjar med "=".

```csharp
public bool HasFormula { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyHasFormulaDemo
    {
        public static void Run()
        {
            // Skapa textläsningsalternativ och aktivera formelparsning
            TxtLoadOptions options = new TxtLoadOptions();
            options.HasFormula = true;
            options.SeparatorString = "|";

            // Läs in arbetsbok med formler i textfilen
            Workbook workbook = new Workbook("example.csv", options);
            
            // Åtkomst till en cell med formel och visa den
            Console.WriteLine("Cell K2 formula: " + workbook.Worksheets[0].Cells["K2"].Formula);
            
            // Spara arbetsboken
            workbook.Save("example_output.xlsx");
        }
    }
}
```

### Se även

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


