---
title: "Column.IsCollapsed"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Kolumnegenskap. om kolumnen är kollapsad"
type: docs
url: /sv/net/aspose.cells/column/iscollapsed/
---
## Column.IsCollapsed property

om kolumnen är hopfälld

```csharp
public bool IsCollapsed { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ColumnPropertyIsCollapsedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa och tillämpa en enkel stil på kolumnen
            Style style = workbook.CreateStyle();
            style.BackgroundColor = Color.LightGray;
            
            Column column = worksheet.Cells.Columns[0];
            column.ApplyStyle(style, new StyleFlag { All = true });

            // Ställ in kolumnegenskaper inklusive IsCollapsed
            column.Width = 15;
            column.IsCollapsed = true; // Demonstrating IsCollapsed property
            column.IsHidden = false;

            // Lägg till lite data för att visualisera den kollapsade kolumnen
            worksheet.Cells["A1"].PutValue("Collapsed Column");
            worksheet.Cells["B1"].PutValue("Visible Column");

            workbook.Save("ColumnIsCollapsedDemo.xlsx");
        }
    }
}
```

### Se även

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


