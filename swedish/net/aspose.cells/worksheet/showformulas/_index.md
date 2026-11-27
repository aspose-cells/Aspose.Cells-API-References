---
title: "Worksheet.ShowFormulas"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Anger om formler eller deras resultat ska visas"
type: docs
url: /sv/net/aspose.cells/worksheet/showformulas/
---
## Worksheet.ShowFormulas property

Anger om formler eller deras resultat ska visas.

```csharp
public bool ShowFormulas { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyShowFormulasDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ställ in formel i cell A1
            worksheet.Cells["A1"].Formula = "=1+2+3";
            
            // Visa beräknat värde initialt
            worksheet.ShowFormulas = false;
            Console.WriteLine("ShowFormulas OFF: " + worksheet.Cells["A1"].StringValue);

            // Växla för att visa formeltext
            worksheet.ShowFormulas = true;
            Console.WriteLine("ShowFormulas ON: " + worksheet.Cells["A1"].StringValue);
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


