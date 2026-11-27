---
title: "Cell.Column"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-egenskap. Hämtar kolumnnummer nollbaserat för cellen"
type: docs
url: /sv/net/aspose.cells/cell/column/
---
## Cell.Column property

Hämtar kolumnnumret (nollbaserat) för cellen.

```csharp
public int Column { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyColumnDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Åtkomst till celler och demonstrera Column-egenskapen
            Cell cell1 = worksheet.Cells["A1"];
            Cell cell2 = worksheet.Cells["B2"];
            Cell cell3 = worksheet.Cells["C3"];

            // Ange värden och format
            cell1.PutValue("Cell A1");
            cell2.PutValue("Cell B2");
            cell3.PutValue("Cell C3");

            // Demonstrera användning av Column-egenskapen
            Console.WriteLine("Cell A1 is in column: " + cell1.Column);
            Console.WriteLine("Cell B2 is in column: " + cell2.Column);
            Console.WriteLine("Cell C3 is in column: " + cell3.Column);

            // Ändra kolumnbredd med Column-egenskapen
            worksheet.Cells.Columns[cell1.Column].Width = 20;
            worksheet.Cells.Columns[cell2.Column].Width = 25;
            worksheet.Cells.Columns[cell3.Column].Width = 30;

            // Spara arbetsboken
            workbook.Save("ColumnPropertyDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


