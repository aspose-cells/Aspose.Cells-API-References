---
title: "CellsHelper.CellIndexToName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellsHelper-metod. Hämtar cellnamn enligt dess rad- och kolumnindex"
type: docs
url: /sv/net/aspose.cells/cellshelper/cellindextoname/
---
## CellsHelper.CellIndexToName method

Hämtar cellnamn enligt dess rad- och kolumnindex.

```csharp
public static string CellIndexToName(int row, int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindex. |
| column | Int32 | Kolumnindex. |

### Returvärde

Cellens namn.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodCellIndexToNameWithInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i lite data
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(20);

            // Hämta cellnamnet från rad- och kolumnindex
            string cellName = CellsHelper.CellIndexToName(2, 1); // Row 2, Column 1 (B3)

            // Skriv ut resultatet
            Console.WriteLine("Cell name for row 2, column 1 is: " + cellName);
        }
    }
}
```

### Se även

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


