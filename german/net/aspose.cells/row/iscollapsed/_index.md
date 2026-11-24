---
title: "Row.IsCollapsed"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Row-Eigenschaft. ob die Zeile zusammengeklappt ist"
type: docs
url: /de/net/aspose.cells/row/iscollapsed/
---
## Row.IsCollapsed property

ob die Zeile zusammengeklappt ist

```csharp
public bool IsCollapsed { get; set; }
```

### Beispiele

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

            // Erstelle und formatiere eine Zeile
            Row row = worksheet.Cells.Rows[0];
            row.Height = 20;
            row.GroupLevel = 1;
            
            // Demonstriere die IsCollapsed-Eigenschaft
            row.IsCollapsed = true;
            Console.WriteLine("Row is collapsed: " + row.IsCollapsed);

            // Erweitere die Zeile
            row.IsCollapsed = false;
            Console.WriteLine("Row is collapsed: " + row.IsCollapsed);

            // Speichere die Arbeitsmappe
            workbook.Save("RowIsCollapsedDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


