---
title: "Column.IsHidden"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Column-egenskap. Anger om kolumnen är dold"
type: docs
url: /sv/net/aspose.cells/column/ishidden/
---
## Column.IsHidden property

Indikerar om kolumnen är dold.

```csharp
public bool IsHidden { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnPropertyIsHiddenDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ange kolumnbredd för demonstration
            worksheet.Cells.Columns[1].Width = 20;
            Console.WriteLine("Column 1 width before hiding: " + worksheet.Cells.Columns[1].Width);

            // Dölj kolumnen
            worksheet.Cells.Columns[1].IsHidden = true;
            Console.WriteLine("Column 1 is hidden: " + worksheet.Cells.Columns[1].IsHidden);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


