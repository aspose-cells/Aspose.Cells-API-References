---
title: "Cells.StandardWidth"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-egenskap. Hämtar eller anger standardkolumnbredd i kalkylbladet i teckenenheter"
type: docs
url: /sv/net/aspose.cells/cells/standardwidth/
---
## Cells.StandardWidth property

Hämtar eller anger standardkolumnbredden i kalkylbladet, i enheten tecken.

```csharp
public double StandardWidth { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardWidthDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ställ in standardbredden för kolumner
            cells.StandardWidth = 18.25;

            // Visa standardbredden och den faktiska bredden för den första kolumnen
            Console.WriteLine("Standard Width: " + cells.StandardWidth);
            Console.WriteLine("Column 0 Width: " + cells.GetColumnWidth(0));

            // Verifiera att standardbredden har tillämpats (ungefärligt)
            if (Math.Abs(cells.GetColumnWidth(0) - cells.StandardWidth) > 1.0)
            {
                Console.WriteLine("Warning: Column width differs significantly from standard width");
            }
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


