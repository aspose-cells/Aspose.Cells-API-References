---
title: "UnionRange.CellCount"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "UnionRange-Eigenschaft. Gibt die gesamte Zellanzahl im Bereich zurück"
type: docs
url: /de/net/aspose.cells/unionrange/cellcount/
---
## UnionRange.CellCount property

Ermittelt die gesamte Zellanzahl im Bereich.

```csharp
public int CellCount { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyCellCountDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Daten im Arbeitsblatt füllen
            for (int row = 0; row < 5; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    worksheet.Cells[row, col].Value = $"Cell {row + 1},{col + 1}";
                }
            }

            // Erstellen Sie Bereiche und kombinieren Sie sie zu einem Union-Bereich
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B3");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("D1:E4");
            UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });

            // Zeige die CellCount-Eigenschaft an
            Console.WriteLine("Total cells in union range: " + unionRange.CellCount);

            // Berechne die erwartete Zellanzahl
            int expectedCount = (range1.RowCount * range1.ColumnCount) + (range2.RowCount * range2.ColumnCount);
            Console.WriteLine("Expected cell count: " + expectedCount);

            // Demonstrieren Sie die Verwendung, indem Sie durch Zellen iterieren
            Console.WriteLine("\nCell values in the union range:");
            int cellCounter = 0;
            foreach (Cell cell in unionRange)
            {
                Console.WriteLine($"Cell {cell.Name}: {cell.Value}");
                cellCounter++;
            }

            // Überprüfen Sie, ob die Zellanzahl mit der Iteration übereinstimmt
            Console.WriteLine($"\nIterated through {cellCounter} cells (should match CellCount)");

            // Erstellen Sie einen weiteren Union-Bereich mit anderen Abmessungen
            Aspose.Cells.Range range3 = worksheet.Cells.CreateRange("A5:E5");
            Aspose.Cells.Range range4 = worksheet.Cells.CreateRange("C1:C5");
            UnionRange unionRange2 = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range3, range4 });

            // Vergleichen Sie die Zellzahlen verschiedener Union-Bereiche
            Console.WriteLine("\nSecond union range cell count: " + unionRange2.CellCount);
            Console.WriteLine("First union range has " + 
                (unionRange.CellCount > unionRange2.CellCount ? "more" : "fewer") + 
                " cells than second union range");

            // Speichere die Arbeitsmappe
            workbook.Save("UnionRangeCellCountDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


