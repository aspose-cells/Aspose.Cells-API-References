---
title: "CellsHelper.ColumnIndexToName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellsHelper-metod. Hämtar kolumnnamn enligt kolumnindex"
type: docs
url: /sv/net/aspose.cells/cellshelper/columnindextoname/
---
## CellsHelper.ColumnIndexToName method

Hämtar kolumnnamn enligt kolumnindex.

```csharp
public static string ColumnIndexToName(int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| column | Int32 | Kolumnindex. |

### Returvärde

Kolumnens namn.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodColumnIndexToNameWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ange värden i celler för att demonstrera konvertering från kolumnindex till namn
            worksheet.Cells["A1"].PutValue("Column Index");
            worksheet.Cells["B1"].PutValue("Column Name");

            // Demonstrera ColumnIndexToName för index 0-4
            for (int i = 0; i < 5; i++)
            {
                worksheet.Cells[i + 1, 0].PutValue(i);
                string columnName = CellsHelper.ColumnIndexToName(i);
                worksheet.Cells[i + 1, 1].PutValue(columnName);
            }

            // Spara arbetsboken
            workbook.Save("ColumnIndexToNameDemo.xlsx");
        }
    }
}
```

### Se även

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


