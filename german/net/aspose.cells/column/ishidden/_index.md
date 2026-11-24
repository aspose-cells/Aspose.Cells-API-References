---
title: "Column.IsHidden"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Column-Eigenschaft. Gibt an, ob die Spalte ausgeblendet ist"
type: docs
url: /de/net/aspose.cells/column/ishidden/
---
## Column.IsHidden property

Gibt an, ob die Spalte ausgeblendet ist.

```csharp
public bool IsHidden { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnPropertyIsHiddenDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Spaltenbreite zur Demonstration festlegen
            worksheet.Cells.Columns[1].Width = 20;
            Console.WriteLine("Column 1 width before hiding: " + worksheet.Cells.Columns[1].Width);

            // Spalte ausblenden
            worksheet.Cells.Columns[1].IsHidden = true;
            Console.WriteLine("Column 1 is hidden: " + worksheet.Cells.Columns[1].IsHidden);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


