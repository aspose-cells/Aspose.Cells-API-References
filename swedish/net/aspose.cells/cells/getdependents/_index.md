---
title: "Cells.GetDependents"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Hämta alla celler som refererar till den specifika cellen"
type: docs
url: /sv/net/aspose.cells/cells/getdependents/
---
## Cells.GetDependents method

Hämta alla celler som refererar till den specifika cellen.

```csharp
public Cell[] GetDependents(bool isAll, int row, int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isAll | Boolean | Anger om andra arbetsblad ska kontrolleras |
| row | Int32 | Radindexet. |
| column | Int32 | Kolumnindexet. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetDependentsWithBooleanInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ställ in exempelformler och värden
            cells["A1"].PutValue(10);
            cells["B1"].Formula = "=A1*2";
            cells["C1"].Formula = "=A1+B1";
            cells["D1"].Formula = "=B1*3";
            cells["F4"].Formula = "=A1*5";

            // Beräkna formler
            workbook.CalculateFormula();

            // Hämta direkta beroenden för cell A1 (rad 0, kolumn 0)
            Cell[] directDependents = cells.GetDependents(false, 0, 0);
            Console.WriteLine("Direct dependents of A1:");
            foreach (Cell cell in directDependents)
            {
                Console.WriteLine(cell.Name);
            }

            // Hämta alla beroenden (inklusive indirekta) för cell A1 (rad 0, kolumn 0)
            Cell[] allDependents = cells.GetDependents(true, 0, 0);
            Console.WriteLine("\nAll dependents of A1:");
            foreach (Cell cell in allDependents)
            {
                Console.WriteLine(cell.Name);
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


