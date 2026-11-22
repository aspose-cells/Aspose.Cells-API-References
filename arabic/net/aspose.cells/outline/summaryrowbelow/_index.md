---
title: "Outline.SummaryRowBelow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Outline. تشير إلى ما إذا كان صف الملخص سيُوضع أسفل صفوف التفاصيل في المخطط"
type: docs
url: /ar/net/aspose.cells/outline/summaryrowbelow/
---
## Outline.SummaryRowBelow property

يشير إلى ما إذا كان سيتم وضع صف الملخص أسفل صفوف التفاصيل في المخطط.

```csharp
public bool SummaryRowBelow { get; set; }
```

### أمثلة

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
            
            // إضافة بيانات تجريبية وتجزئة
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("Total");
            worksheet.Cells["B4"].PutValue("=SUM(B2:B3)");
            
            // تجميع الصفوف وتعيين موضع صف الملخص
            worksheet.Cells.GroupRows(1, 2, false);
            Outline outline = worksheet.Outline;
            outline.SummaryRowBelow = true;
            
            workbook.Save("OutlineSummaryRowBelow.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Outline](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


