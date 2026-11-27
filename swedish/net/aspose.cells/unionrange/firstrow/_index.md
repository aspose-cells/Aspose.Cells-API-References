---
title: "UnionRange.FirstRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "UnionRange-egenskap. Hämtar indexet för den första raden i intervallet"
type: docs
url: /sv/net/aspose.cells/unionrange/firstrow/
---
## UnionRange.FirstRow property

Hämtar indexet för den första raden i området.

```csharp
public int FirstRow { get; }
```

### Anmärkningar

Påverkar endast när den bara innehåller ett område.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyFirstRowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i exempeldata
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    worksheet.Cells[row, col].Value = $"Row {row}, Col {col}";
                }
            }

            // Skapa ett unionområde från A2:C5 och A7:C9
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A2:C5");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A7:C9");
            UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });

            // Visa egenskapen FirstRow
            Console.WriteLine("FirstRow of union range: " + unionRange.FirstRow);

            // Visa användning genom att markera den första raden
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

            // Skapa ett annat område och jämför FirstRow‑värden
            Aspose.Cells.Range singleRange = worksheet.Cells.CreateRange("D1:F5");
            Console.WriteLine("FirstRow of single range: " + singleRange.FirstRow);
            Console.WriteLine("Is union range starting after single range? " + 
                (unionRange.FirstRow > singleRange.FirstRow));

            // Spara arbetsboken
            workbook.Save("UnionRangeFirstRowDemo.xlsx");
        }
    }
}
```

### Se även

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


