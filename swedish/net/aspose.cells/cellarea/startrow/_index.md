---
title: "CellArea.StartRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellArea-fält. Hämtar eller ange startraden i detta område"
type: docs
url: /sv/net/aspose.cells/cellarea/startrow/
---
## CellArea.StartRow field

Hämtar eller anger startraden för detta område.

```csharp
public int StartRow;
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaFieldStartRowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa två CellArea-objekt
            CellArea area1 = new CellArea();
            area1.StartRow = 2;
            area1.StartColumn = 1;
            area1.EndRow = 5;
            area1.EndColumn = 3;

            CellArea area2 = new CellArea();
            area2.StartRow = area1.StartRow; // Demonstrating StartRow usage
            area2.StartColumn = area1.StartColumn;
            area2.EndRow = area1.EndRow;
            area2.EndColumn = area1.EndColumn;

            // Verifiera att områdena matchar
            if (area1.StartRow == area2.StartRow &&
                area1.StartColumn == area2.StartColumn &&
                area1.EndRow == area2.EndRow &&
                area1.EndColumn == area2.EndColumn)
            {
                Console.WriteLine("CellArea objects match successfully");
                Console.WriteLine($"StartRow: {area1.StartRow}");
            }
            else
            {
                Console.WriteLine("CellArea objects do not match");
            }
        }
    }
}
```

### Se även

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


