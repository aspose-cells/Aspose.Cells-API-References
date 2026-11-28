---
title: "Outline.SummaryRowBelow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Outline özelliği. Özet satırının, ana hatta detay satırlarının altında konumlandırılıp konumlandırılmayacağını gösterir"
type: docs
url: /tr/net/aspose.cells/outline/summaryrowbelow/
---
## Outline.SummaryRowBelow property

Anahattaki özet satırının detay satırlarının altında konumlandırılıp konumlandırılmayacağını gösterir.

```csharp
public bool SummaryRowBelow { get; set; }
```

### Örnekler

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
            
            // Örnek veri ve gruplama ekle
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("Total");
            worksheet.Cells["B4"].PutValue("=SUM(B2:B3)");
            
            // Satırları grupla ve özet satırının konumunu ayarla
            worksheet.Cells.GroupRows(1, 2, false);
            Outline outline = worksheet.Outline;
            outline.SummaryRowBelow = true;
            
            workbook.Save("OutlineSummaryRowBelow.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Outline](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


