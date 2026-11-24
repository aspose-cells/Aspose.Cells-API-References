---
title: "Range.ColumnCount"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Eigenschaft. Gibt die Anzahl der Spalten im Bereich zurück"
type: docs
url: /de/net/aspose.cells/range/columncount/
---
## Range.ColumnCount property

Liefert die Anzahl der Spalten im Bereich.

```csharp
public int ColumnCount { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyColumnCountDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet sheet = workbook.Worksheets[0];
            
            // Erstelle Beispieldaten (5 Spalten x 3 Zeilen)
            for (int col = 0; col < 5; col++)
            {
                for (int row = 0; row < 3; row++)
                {
                    sheet.Cells[row, col].PutValue($"Data {row},{col}");
                }
            }
            
            // Erstelle einen Bereich, der alle Datenspalten abdeckt
            Aspose.Cells.Range dataRange = sheet.Cells.CreateRange(0, 0, 3, 5);
            
            // Demonstriere die Verwendung von ColumnCount
            Console.WriteLine($"Range has {dataRange.ColumnCount} columns");
            
            // Passe jede Spalte im Bereich automatisch an
            for (int i = 0; i < dataRange.ColumnCount; i++)
            {
                sheet.AutoFitColumn(dataRange.FirstColumn + i);
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


