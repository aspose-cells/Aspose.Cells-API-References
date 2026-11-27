---
title: "Cells.StandardHeightInch"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-egenskap. Hämtar eller anger standardradhöjden i detta kalkylblad i tum"
type: docs
url: /sv/net/aspose.cells/cells/standardheightinch/
---
## Cells.StandardHeightInch property

Hämtar eller anger standardradshöjden i detta kalkylblad, i enheten tum.

```csharp
public double StandardHeightInch { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardHeightInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hämta standardhöjden i tum
            double standardHeightInch = worksheet.Cells.StandardHeightInch;
            Console.WriteLine("Standard Height in Inches: " + standardHeightInch);
            
            // Ställ in en ny standardhöjd (1 tum)
            worksheet.Cells.StandardHeightInch = 1.0;
            Console.WriteLine("New Standard Height in Inches: " + worksheet.Cells.StandardHeightInch);
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


