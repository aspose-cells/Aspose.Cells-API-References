---
title: "UnionRange.FirstRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "UnionRange-Eigenschaft. Gibt den Index der ersten Zeile des Bereichs zurück"
type: docs
url: /de/net/aspose.cells/unionrange/firstrow/
---
## UnionRange.FirstRow property

Liefert den Index der ersten Zeile des Bereichs.

```csharp
public int FirstRow { get; }
```

### Hinweise

Nur wirksam, wenn es nur einen Bereich enthält.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyFirstRowDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten befüllen
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    worksheet.Cells[row, col].Value = $"Row {row}, Col {col}";
                }
            }

            // Erstelle einen Union-Bereich aus A2:C5 und A7:C9
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A2:C5");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A7:C9");
            UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });

            // Zeige die FirstRow-Eigenschaft an
            Console.WriteLine("FirstRow of union range: " + unionRange.FirstRow);

            // Demonstrieren Sie die Verwendung, indem Sie die erste Zeile hervorheben
            Style highlightStyle = workbook.CreateStyle();
            highlightStyle.Font.IsBold = true;
            highlightStyle.ForegroundColor = System.Drawing.Color.LightGreen;
            highlightStyle.Pattern = BackgroundType.Solid;

            Aspose.Cells.Range firstRowRange = worksheet.Cells.CreateRange(
                unionRange.FirstRow,
                unionRange.FirstColumn,
                1,
                unionRange.ColumnCount);
            firstRowRange.ApplyStyle(highlightStyle, new StyleFlag { FontBold = true, CellShading = true });

            // Erstellen Sie einen weiteren Bereich und vergleichen Sie die Werte von FirstRow
            Aspose.Cells.Range singleRange = worksheet.Cells.CreateRange("D1:F5");
            Console.WriteLine("FirstRow of single range: " + singleRange.FirstRow);
            Console.WriteLine("Is union range starting after single range? " + 
                (unionRange.FirstRow > singleRange.FirstRow));

            // Speichere die Arbeitsmappe
            workbook.Save("UnionRangeFirstRowDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


