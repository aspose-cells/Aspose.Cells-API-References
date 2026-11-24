---
title: "Range.FirstColumn"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Eigenschaft. Gibt den Index der ersten Spalte des Bereichs zurück"
type: docs
url: /de/net/aspose.cells/range/firstcolumn/
---
## Range.FirstColumn property

Liefert den Index der ersten Spalte des Bereichs.

```csharp
public int FirstColumn { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyFirstColumnDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle Beispieldaten
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);

            // Erstelle einen Bereich
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B2");

            // Demonstrieren Sie die FirstColumn-Eigenschaft
            Console.WriteLine("First column index of range: " + range.FirstColumn);

            // Verwenden Sie FirstColumn, um auf Zellen in der ersten Spalte des Bereichs zuzugreifen
            for (int i = 0; i < range.RowCount; i++)
            {
                Cell cell = range[i, 0]; // Access first column (index 0) of the range
                Console.WriteLine($"Cell[{i},0] value: {cell.StringValue}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("RangeFirstColumnDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


