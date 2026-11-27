---
title: "Cells.MaxDataRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-egenskap. Maximalt radindex för cell som innehåller data"
type: docs
url: /sv/net/aspose.cells/cells/maxdatarow/
---
## Cells.MaxDataRow property

Maximalt radindex för celler som innehåller data.

```csharp
public int MaxDataRow { get; }
```

### Anmärkningar

Returnera -1 om det inte finns någon cell som innehåller data. Denna egenskap måste iterera och kontrollera celler och rader dynamiskt, så det är en tidskrävande process och bör inte anropas upprepade gånger, till exempel genom att använda den direkt som villkor i en loop.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxDataRowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("Item1");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("Item2");
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["A4"].PutValue("Item3");
            sheet.Cells["B4"].PutValue(30);

            // Demonstrera användning av MaxDataRow
            int maxRow = sheet.Cells.MaxDataRow;
            Console.WriteLine("Max data row: " + maxRow);

            // Skapa ett cellområde med MaxDataRow
            int startRow = 0;
            int startColumn = 0;
            int endRow = sheet.Cells.MaxDataRow;
            int endColumn = sheet.Cells.MaxDataColumn;

            // Tillämpa formatering på dataområdet
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            
            // Applicera stil på området
            sheet.Cells.CreateRange(startRow, startColumn, endRow + 1, endColumn + 1).ApplyStyle(style, new StyleFlag { FontBold = true });

            // Spara arbetsboken
            workbook.Save("MaxDataRowDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


