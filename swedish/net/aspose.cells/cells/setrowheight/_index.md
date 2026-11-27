---
title: "Cells.SetRowHeight"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Anger höjden på den angivna raden"
type: docs
url: /sv/net/aspose.cells/cells/setrowheight/
---
## Cells.SetRowHeight method

Ställer in höjden på den angivna raden.

```csharp
public void SetRowHeight(int row, double height)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindex. |
| höjd | Double | Radens höjd. I enheten punkt. Den bör vara mellan 0 och 409.5. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetRowHeightWithInt32DoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ange radens höjd för första raden (index 0) till 25.5 punkter
            cells.SetRowHeight(0, 25.5);

            // Verifiera radens höjd
            Console.WriteLine("Row height of row 0: " + cells.GetRowHeight(0));
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


