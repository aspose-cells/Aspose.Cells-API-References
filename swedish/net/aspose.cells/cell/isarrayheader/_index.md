---
title: "Cell.IsArrayHeader"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell egenskap. Anger att cellens formel är en matrisformel och att den är den första cellen i matrisen"
type: docs
url: /sv/net/aspose.cells/cell/isarrayheader/
---
## Cell.IsArrayHeader property

Anger att cellens formel är en matrisformel och att den är den första cellen i matrisen.

```csharp
public bool IsArrayHeader { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsArrayHeaderDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa en matrisformel i området B2:D4
            worksheet.Cells["B2"].SetArrayFormula("=A1:A3*B1:B3", 3, 3);
            
            // Verifiera och skriv ut egenskapen IsArrayHeader
            // Obs: IsArrayHeader är skrivskyddad och sätts automatiskt för matrisformelrubriker
            Console.WriteLine("B2 IsArrayHeader: " + worksheet.Cells["B2"].IsArrayHeader);
            Console.WriteLine("B3 IsArrayHeader: " + worksheet.Cells["B3"].IsArrayHeader);
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


