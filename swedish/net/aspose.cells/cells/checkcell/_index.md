---
title: "Cells.CheckCell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Hämtar Cell-elementet eller null på det angivna cellradindexet och kolumnindexet"
type: docs
url: /sv/net/aspose.cells/cells/checkcell/
---
## Cells.CheckCell method

Hämtar [`Cell`](../../cell/) elementet eller null på det angivna cellradindexet och kolumnindexet.

```csharp
public Cell CheckCell(int row, int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindex |
| column | Int32 | Kolumnindex |

### Returvärde

Returnera Cell-objektet om ett Cell-objekt finns. Returnera null om cellen inte finns.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCheckCellWithInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ange värden i cells
            cells[0, 0].PutValue("Hello");
            cells[1, 1].PutValue(123);
            cells[2, 2].PutValue(DateTime.Now);

            // Kontrollera celler med CheckCell-metoden med Int32-parametrar
            Cell cell1 = cells.CheckCell(0, 0);
            Console.WriteLine("Cell A1 value: " + cell1.StringValue);

            Cell cell2 = cells.CheckCell(1, 1);
            Console.WriteLine("Cell B2 value: " + cell2.StringValue);

            Cell cell3 = cells.CheckCell(2, 2);
            Console.WriteLine("Cell C3 value: " + cell3.StringValue);

            // Kontrollera icke-existerande cell (returnerar null)
            Cell cell4 = cells.CheckCell(10, 10);
            if (cell4 == null)
            {
                Console.WriteLine("Cell K11 doesn't exist (as expected)");
            }
        }
    }
}
```

### Se även

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


