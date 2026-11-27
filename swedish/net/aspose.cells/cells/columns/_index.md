---
title: "Cells.Columns"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-egenskap. Hämtar samlingen av Column-objekt som representerar de enskilda kolumnerna i detta kalkylblad"
type: docs
url: /sv/net/aspose.cells/cells/columns/
---
## Cells.Columns property

Hämtar samlingen av [`Column`](../../column/) objekt som representerar de enskilda kolumnerna i detta kalkylblad.

```csharp
public ColumnCollection Columns { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyColumnsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ange stil för kolumn 5
            Style columnStyle = workbook.CreateStyle();
            columnStyle.Font.Name = "Arial";
            columnStyle.Font.Size = 12;
            columnStyle.Font.IsBold = true;
            cells.Columns[5].ApplyStyle(columnStyle, new StyleFlag { FontName = true, FontSize = true, FontBold = true });

            // Ange bredd för kolumn 5
            cells.Columns[5].Width = 20;

            // Ange data i kolumn 5 för att demonstrera stilen
            for (int row = 0; row < 10; row++)
            {
                cells[row, 5].PutValue($"Row {row + 1}");
            }

            // Spara arbetsboken
            workbook.Save("ColumnsPropertyDemo.xlsx");
        }
    }
}
```

### Se även

* class [ColumnCollection](../../columncollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


