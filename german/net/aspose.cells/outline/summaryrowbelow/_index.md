---
title: "Outline.SummaryRowBelow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Outline-Eigenschaft. Gibt an, ob die Zusammenfassungszeile unter den Detailzeilen in der Gliederung positioniert wird"
type: docs
url: /de/net/aspose.cells/outline/summaryrowbelow/
---
## Outline.SummaryRowBelow property

Gibt an, ob die Zusammenfassungszeile unter den Detailzeilen in der Gliederung positioniert wird.

```csharp
public bool SummaryRowBelow { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OutlinePropertySummaryRowBelowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten und Gruppierung hinzufügen
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("Total");
            worksheet.Cells["B4"].PutValue("=SUM(B2:B3)");
            
            // Zeilen gruppieren und Position der Zusammenfassungszeile festlegen
            worksheet.Cells.GroupRows(1, 2, false);
            Outline outline = worksheet.Outline;
            outline.SummaryRowBelow = true;
            
            workbook.Save("OutlineSummaryRowBelow.xlsx");
        }
    }
}
```

### Siehe auch

* class [Outline](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


