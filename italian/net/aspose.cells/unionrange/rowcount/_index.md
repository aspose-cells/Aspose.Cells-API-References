---
title: "UnionRange.RowCount"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà UnionRange. Restituisce il conteggio delle righe nell'intervallo"
type: docs
url: /it/net/aspose.cells/unionrange/rowcount/
---
## UnionRange.RowCount property

Ottiene il conteggio delle righe nell'intervallo.

```csharp
public int RowCount { get; }
```

### Osservazioni

Ha effetto solo quando contiene un solo intervallo.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyRowCountDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola i dati nel foglio di lavoro
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    worksheet.Cells[row, col].Value = $"Data {row},{col}";
                }
            }

            // Crea un intervallo di unione da A1 a E5
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:E5");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A6:E10");
            UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });

            // Visualizza la proprietà RowCount
            Console.WriteLine("RowCount of union range: " + unionRange.RowCount);

            // Dimostra l'uso iterando attraverso le righe
            for (int i = 0; i < unionRange.RowCount; i++)
            {
                Aspose.Cells.Range currentRow = worksheet.Cells.CreateRange(
                    unionRange.FirstRow + i,
                    unionRange.FirstColumn,
                    1,
                    unionRange.ColumnCount);

                Console.WriteLine($"Row {i + 1} first cell value: " + currentRow[0, 0].Value);
            }

            // Crea un nuovo intervallo con un diverso conteggio di righe
            Aspose.Cells.Range newRange = worksheet.Cells.CreateRange("A1:E3");
            Console.WriteLine("RowCount of new range: " + newRange.RowCount);

            // Applica la formattazione basata sul conteggio delle righe
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

            // Salva la cartella di lavoro
            workbook.Save("UnionRangeRowCountDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


