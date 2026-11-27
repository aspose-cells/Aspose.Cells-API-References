---
title: "Row.IsCollapsed"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Row-egenskap. Anger om raden är kollapsad"
type: docs
url: /sv/net/aspose.cells/row/iscollapsed/
---
## Row.IsCollapsed property

om raden är hopfälld

```csharp
public bool IsCollapsed { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyIsCollapsedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa och formatera en rad
            Row row = worksheet.Cells.Rows[0];
            row.Height = 20;
            row.GroupLevel = 1;
            
            // Demonstrera IsCollapsed-egenskapen
            row.IsCollapsed = true;
            Console.WriteLine("Row is collapsed: " + row.IsCollapsed);

            // Expandera raden
            row.IsCollapsed = false;
            Console.WriteLine("Row is collapsed: " + row.IsCollapsed);

            // Spara arbetsboken
            workbook.Save("RowIsCollapsedDemo.xlsx");
        }
    }
}
```

### Se även

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


