---
title: "Column.IsCollapsed"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Column. indica se la colonna è compressa"
type: docs
url: /it/net/aspose.cells/column/iscollapsed/
---
## Column.IsCollapsed property

se la colonna è compressa

```csharp
public bool IsCollapsed { get; set; }
```

### Esempi

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

            // Crea e applica uno stile semplice alla colonna
            Style style = workbook.CreateStyle();
            style.BackgroundColor = Color.LightGray;
            
            Column column = worksheet.Cells.Columns[0];
            column.ApplyStyle(style, new StyleFlag { All = true });

            // Imposta le proprietà della colonna includendo IsCollapsed
            column.Width = 15;
            column.IsCollapsed = true; // Demonstrating IsCollapsed property
            column.IsHidden = false;

            // Aggiungi alcuni dati per visualizzare la colonna compressa
            worksheet.Cells["A1"].PutValue("Collapsed Column");
            worksheet.Cells["B1"].PutValue("Visible Column");

            workbook.Save("ColumnIsCollapsedDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


