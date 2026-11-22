---
title: "AutoFilter.Range"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AutoFilter. تمثل النطاق الذي يُطبق عليه AutoFilter المحدد"
type: docs
url: /ar/net/aspose.cells/autofilter/range/
---
## AutoFilter.Range property

يمثل النطاق الذي ينطبق عليه AutoFilter المحدد.

```csharp
public string Range { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterPropertyRangeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue("Header");
            sheet.Cells["A2"].PutValue("Item1");
            sheet.Cells["A3"].PutValue("Item2");
            sheet.Cells["A4"].PutValue("Item3");
            sheet.Cells["A5"].PutValue("Item4");

            // تطبيق الفلتر التلقائي على النطاق A1:A5
            sheet.AutoFilter.Range = "A1:A5";

            // عرض نطاق الفلتر التلقائي
            Console.WriteLine("AutoFilter Range: " + sheet.AutoFilter.Range);

            // احفظ المصنف
            workbook.Save("AutoFilterRangeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


