---
title: "Column.Index"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Column-Eigenschaft. Gibt den Index dieser Spalte zurück"
type: docs
url: /de/net/aspose.cells/column/index/
---
## Column.Index property

Ermittelt den Index dieser Spalte.

```csharp
public int Index { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnPropertyIndexDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge einige Daten zu den Spalten hinzu
            worksheet.Cells["A1"].PutValue("Column 1");
            worksheet.Cells["B1"].PutValue("Column 2");
            worksheet.Cells["C1"].PutValue("Column 3");
            
            // Rufe die Spaltensammlung ab
            ColumnCollection columns = worksheet.Cells.Columns;
            
            // Demonstriere die Index-Eigenschaft
            Console.WriteLine("Column Indices:");
            for (int i = 0; i < columns.Count; i++)
            {
                Column column = columns[i];
                Console.WriteLine($"Column {column.Index}: {worksheet.Cells[0, column.Index].StringValue}");
            }
            
            // Greife per Index auf die Spalte zu
            Column columnB = columns[1]; // B column (index 1)
            Console.WriteLine($"\nAccessed by index 1: {worksheet.Cells[0, columnB.Index].StringValue}");
            
            // Ändere die Spaltenbreite mittels Index
            columns[2].Width = 30; // C column (index 2)
            Console.WriteLine($"\nColumn C width set to: {columns[2].Width}");
        }
    }
}
```

### Siehe auch

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


