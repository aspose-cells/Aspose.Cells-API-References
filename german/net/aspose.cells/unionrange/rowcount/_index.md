---
title: "UnionRange.RowCount"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "UnionRange-Eigenschaft. Gibt die Anzahl der Zeilen im Bereich zurück"
type: docs
url: /de/net/aspose.cells/unionrange/rowcount/
---
## UnionRange.RowCount property

Liefert die Anzahl der Zeilen im Bereich.

```csharp
public int RowCount { get; }
```

### Hinweise

Nur wirksam, wenn es nur einen Bereich enthält.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyRowCountDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Daten im Arbeitsblatt füllen
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    worksheet.Cells[row, col].Value = $"Data {row},{col}";
                }
            }

            // Erstellen Sie einen Union-Bereich von A1 bis E5
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:E5");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A6:E10");
            UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });

            // Zeige die RowCount-Eigenschaft an
            Console.WriteLine("RowCount of union range: " + unionRange.RowCount);

            // Demonstrieren Sie die Verwendung, indem Sie durch Zeilen iterieren
            for (int i = 0; i < unionRange.RowCount; i++)
            {
                Aspose.Cells.Range currentRow = worksheet.Cells.CreateRange(
                    unionRange.FirstRow + i,
                    unionRange.FirstColumn,
                    1,
                    unionRange.ColumnCount);

                Console.WriteLine($"Row {i + 1} first cell value: " + currentRow[0, 0].Value);
            }

            // Erstellen Sie einen neuen Bereich mit unterschiedlicher Zeilenanzahl
            Aspose.Cells.Range newRange = worksheet.Cells.CreateRange("A1:E3");
            Console.WriteLine("RowCount of new range: " + newRange.RowCount);

            // Wenden Sie die Formatierung basierend auf der Zeilenanzahl an
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightYellow;
            style.Pattern = BackgroundType.Solid;

            for (int i = 0; i < unionRange.RowCount; i += 2)
            {
                Aspose.Cells.Range rowRange = worksheet.Cells.CreateRange(
                    unionRange.FirstRow + i,
                    unionRange.FirstColumn,
                    1,
                    unionRange.ColumnCount);
                rowRange.ApplyStyle(style, new StyleFlag { FontBold = true, CellShading = true });
            }

            // Speichere die Arbeitsmappe
            workbook.Save("UnionRangeRowCountDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


