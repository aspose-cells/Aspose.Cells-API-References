---
title: "Outline.SummaryRowBelow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Outline-egenskap. Anger om sammanfattningsraden ska placeras under detaljraderna i dispositionen"
type: docs
url: /sv/net/aspose.cells/outline/summaryrowbelow/
---
## Outline.SummaryRowBelow property

Anger om sammanfattningsraden kommer att placeras under detaljraderna i konturen.

```csharp
public bool SummaryRowBelow { get; set; }
```

### Exempel

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
            
            // Lägg till exempeldata och gruppering
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("Total");
            worksheet.Cells["B4"].PutValue("=SUM(B2:B3)");
            
            // Gruppera rader och ange position för sammanfattningsrad
            worksheet.Cells.GroupRows(1, 2, false);
            Outline outline = worksheet.Outline;
            outline.SummaryRowBelow = true;
            
            workbook.Save("OutlineSummaryRowBelow.xlsx");
        }
    }
}
```

### Se även

* class [Outline](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


