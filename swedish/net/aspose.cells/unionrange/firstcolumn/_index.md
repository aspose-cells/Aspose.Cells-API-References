---
title: "UnionRange.FirstColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "UnionRange‑egenskap. Hämtar indexet för den första kolumnen i området"
type: docs
url: /sv/net/aspose.cells/unionrange/firstcolumn/
---
## UnionRange.FirstColumn property

Hämtar indexet för den första kolumnen i området.

```csharp
public int FirstColumn { get; }
```

### Anmärkningar

Påverkar endast när den bara innehåller ett område.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyFirstColumnDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i lite data
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["C1"].PutValue("Header3");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            worksheet.Cells["C2"].PutValue("Data3");

            // Skapa ett union‑område
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:C1");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A2:C2");
            UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });

            // Visa FirstColumn‑egenskapen
            Console.WriteLine("First column index of the union range: " + unionRange.FirstColumn);

            // Visa användning av FirstColumn i operationer
            Console.WriteLine("First column name: " + CellsHelper.ColumnIndexToName(unionRange.FirstColumn));

            // Applicera formatering på den första kolumnen i unionområdet
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightGray;
            style.Pattern = BackgroundType.Solid;

            Aspose.Cells.Range firstColumnRange = worksheet.Cells.CreateRange(
                unionRange.FirstRow, unionRange.FirstColumn,
                unionRange.RowCount, 1);
            firstColumnRange.ApplyStyle(style, new StyleFlag { FontBold = true, CellShading = true });

            // Spara resultatet
            workbook.Save("UnionRangePropertyFirstColumnDemo.xlsx");
        }
    }
}
```

### Se även

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


