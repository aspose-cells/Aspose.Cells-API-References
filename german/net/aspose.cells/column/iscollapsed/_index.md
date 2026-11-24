---
title: "Column.IsCollapsed"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Column-Eigenschaft. ob die Spalte zusammengeklappt ist"
type: docs
url: /de/net/aspose.cells/column/iscollapsed/
---
## Column.IsCollapsed property

ob die Spalte zusammengeklappt ist

```csharp
public bool IsCollapsed { get; set; }
```

### Beispiele

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

            // Erstelle und wende einen einfachen Stil auf die Spalte an
            Style style = workbook.CreateStyle();
            style.BackgroundColor = Color.LightGray;
            
            Column column = worksheet.Cells.Columns[0];
            column.ApplyStyle(style, new StyleFlag { All = true });

            // Setze Spalteneigenschaften einschließlich IsCollapsed
            column.Width = 15;
            column.IsCollapsed = true; // Demonstrating IsCollapsed property
            column.IsHidden = false;

            // Füge einige Daten hinzu, um die zusammengeklappte Spalte zu visualisieren
            worksheet.Cells["A1"].PutValue("Collapsed Column");
            worksheet.Cells["B1"].PutValue("Visible Column");

            workbook.Save("ColumnIsCollapsedDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


