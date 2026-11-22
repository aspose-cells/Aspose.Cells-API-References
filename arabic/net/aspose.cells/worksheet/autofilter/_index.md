---
title: "Worksheet.AutoFilter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. تمثل الفلتر التلقائي للورقة المحددة"
type: docs
url: /ar/net/aspose.cells/worksheet/autofilter/
---
## Worksheet.AutoFilter property

يمثل الفلتر التلقائي للورقة المحددة.

```csharp
public AutoFilter AutoFilter { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyAutoFilterDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue("Electronics");
            worksheet.Cells["A3"].PutValue("Shirt");
            worksheet.Cells["B3"].PutValue("Clothing");
            worksheet.Cells["A4"].PutValue("Phone");
            worksheet.Cells["B4"].PutValue("Electronics");
            worksheet.Cells["A5"].PutValue("Pants");
            worksheet.Cells["B5"].PutValue("Clothing");

            // تطبيق الفلتر التلقائي
            worksheet.AutoFilter.Range = "A1:B5";
            worksheet.AutoFilter.Filter(1, "Electronics");

            // تحديث الفلتر
            worksheet.AutoFilter.Refresh();

            // احفظ المصنف
            workbook.Save("AutoFilterDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [AutoFilter](../../autofilter/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


