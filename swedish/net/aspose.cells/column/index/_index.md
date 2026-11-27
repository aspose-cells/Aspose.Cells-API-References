---
title: "Column.Index"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Kolumnegenskap. Hämtar indexet för den här kolumnen"
type: docs
url: /sv/net/aspose.cells/column/index/
---
## Column.Index property

Hämtar indexet för den här kolumnen.

```csharp
public int Index { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnPropertyIndexDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till lite data i kolumnerna
            worksheet.Cells["A1"].PutValue("Column 1");
            worksheet.Cells["B1"].PutValue("Column 2");
            worksheet.Cells["C1"].PutValue("Column 3");
            
            // Hämta kolumnsamlingen
            ColumnCollection columns = worksheet.Cells.Columns;
            
            // Demonstrera Index‑egenskapen
            Console.WriteLine("Column Indices:");
            for (int i = 0; i < columns.Count; i++)
            {
                Column column = columns[i];
                Console.WriteLine($"Column {column.Index}: {worksheet.Cells[0, column.Index].StringValue}");
            }
            
            // Åtkomst till kolumn via index
            Column columnB = columns[1]; // B column (index 1)
            Console.WriteLine($"\nAccessed by index 1: {worksheet.Cells[0, columnB.Index].StringValue}");
            
            // Ändra kolumnbredd med hjälp av index
            columns[2].Width = 30; // C column (index 2)
            Console.WriteLine($"\nColumn C width set to: {columns[2].Width}");
        }
    }
}
```

### Se även

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


