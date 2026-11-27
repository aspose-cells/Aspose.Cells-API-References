---
title: "Cell.Copy"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-metod. Kopierar data från en källcell"
type: docs
url: /sv/net/aspose.cells/cell/copy/
---
## Cell.Copy method

Kopierar data från en källcell.

```csharp
public void Copy(Cell cell)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cell | Cell | Källa [`Cell`](../) objekt. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodCopyWithCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ställ in värden och stilar i källcellen
            Cell sourceCell = cells["A1"];
            sourceCell.PutValue("Source Value");
            sourceCell.GetStyle().Font.IsBold = true;

            // Skapa destinationscell
            Cell destCell = cells["B1"];

            // Kopiera från källa till destination
            destCell.Copy(sourceCell);

            // Verifiera kopian
            Console.WriteLine("Destination cell value: " + destCell.StringValue);
            Console.WriteLine("Destination cell bold status: " + destCell.GetStyle().Font.IsBold);
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


