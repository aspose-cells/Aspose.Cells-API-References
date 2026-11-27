---
title: "Cells.MaxDisplayRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-egenskap. Hämtar det maximala området som inkluderar data, sammanslagna celler och former"
type: docs
url: /sv/net/aspose.cells/cells/maxdisplayrange/
---
## Cells.MaxDisplayRange property

Hämtar det maximala området som inkluderar data, sammanslagna celler och former.

```csharp
public Range MaxDisplayRange { get; }
```

### Anmärkningar

Returnerar null om kalkylbladet är tomt sedan Aspose.Cells 21.5.2.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxDisplayRangeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data i celler för att skapa ett visningsområde
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["A3"].PutValue(300);
            worksheet.Cells["B3"].PutValue(400);

            // Hämta det maximala visningsområdet
            Aspose.Cells.Range maxDisplayRange = worksheet.Cells.MaxDisplayRange;

            // Skriv ut områdesinformationen
            Console.WriteLine("Max Display Range:");
            Console.WriteLine($"Start Row: {maxDisplayRange.FirstRow}");
            Console.WriteLine($"Start Column: {maxDisplayRange.FirstColumn}");
            Console.WriteLine($"Total Rows: {maxDisplayRange.RowCount}");
            Console.WriteLine($"Total Columns: {maxDisplayRange.ColumnCount}");

            // Skapa ett nytt område baserat på dimensionerna för det maximala visningsområdet
            Aspose.Cells.Range customRange = worksheet.Cells.CreateRange(
                maxDisplayRange.FirstRow,
                maxDisplayRange.FirstColumn,
                maxDisplayRange.RowCount,
                maxDisplayRange.ColumnCount);

            // Tillämpa formatering på området
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightGray;
            style.Pattern = BackgroundType.Solid;
            customRange.ApplyStyle(style, new StyleFlag { FontBold = true, CellShading = true });

            // Spara arbetsboken
            workbook.Save("MaxDisplayRangeDemo.xlsx");
        }
    }
}
```

### Se även

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


