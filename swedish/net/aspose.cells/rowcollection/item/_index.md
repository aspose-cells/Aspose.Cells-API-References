---
title: "RowCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RowCollection-egenskap. Hämtar ett Row-objekt med angivet radindex. Row-objektet för det angivna radindexet kommer att instansieras om det inte redan finns."
type: docs
url: /sv/net/aspose.cells/rowcollection/item/
---
## RowCollection indexer

Hämtar ett [`Row`](../../row/)‑objekt med angivet radindex. Row‑objektet för det angivna radindexet kommer att instansieras om det inte redan finns.

```csharp
public Row this[int rowIndex] { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ange standardbredd för kolumner
            cells.StandardWidth = 20.0;

            // Åtkomst och formatering av rader med Item‑egenskapen
            for (int i = 0; i < 5; i++)
            {
                Row row = cells.Rows[i]; // Using Item property
                Style rowStyle = workbook.CreateStyle();
                rowStyle.Font.IsBold = true;
                rowStyle.Font.Color = System.Drawing.Color.Blue;
                row.ApplyStyle(rowStyle, new StyleFlag { Font = true });
                
                // Åtkomst och formatering av cell i raden
                Cell cell = cells[i, i]; // Using Cells indexer instead of row[i]
                cell.PutValue($"Row {i}, Col {i}");
                Style cellStyle = workbook.CreateStyle();
                cellStyle.BackgroundColor = System.Drawing.Color.LightYellow;
                cell.SetStyle(cellStyle);
            }

            // Spara arbetsboken
            workbook.Save("RowCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Se även

* class [Row](../../row/)
* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


