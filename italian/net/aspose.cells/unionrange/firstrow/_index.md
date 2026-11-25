---
title: "UnionRange.FirstRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà UnionRange. Restituisce l'indice della prima riga dell'intervallo"
type: docs
url: /it/net/aspose.cells/unionrange/firstrow/
---
## UnionRange.FirstRow property

Ottiene l'indice della prima riga dell'intervallo.

```csharp
public int FirstRow { get; }
```

### Osservazioni

Ha effetto solo quando contiene un solo intervallo.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyFirstRowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola dati di esempio
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    worksheet.Cells[row, col].Value = $"Row {row}, Col {col}";
                }
            }

            // Crea un intervallo di unione da A2:C5 e A7:C9
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A2:C5");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A7:C9");
            UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });

            // Visualizza la proprietà FirstRow
            Console.WriteLine("FirstRow of union range: " + unionRange.FirstRow);

            // Dimostra l'uso evidenziando la prima riga
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

            // Crea un altro intervallo e confronta i valori di FirstRow
            Aspose.Cells.Range singleRange = worksheet.Cells.CreateRange("D1:F5");
            Console.WriteLine("FirstRow of single range: " + singleRange.FirstRow);
            Console.WriteLine("Is union range starting after single range? " + 
                (unionRange.FirstRow > singleRange.FirstRow));

            // Salva la cartella di lavoro
            workbook.Save("UnionRangeFirstRowDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


