---
title: "AutoFilter.Sorter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AutoFilter. يحصل على مُرتب البيانات"
type: docs
url: /ar/net/aspose.cells/autofilter/sorter/
---
## AutoFilter.Sorter property

يحصل على مُرتّب البيانات.

```csharp
public DataSorter Sorter { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterPropertySorterDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("C");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("A");
            worksheet.Cells["B3"].PutValue(10);
            worksheet.Cells["A4"].PutValue("B");
            worksheet.Cells["B4"].PutValue(20);

            // إنشاء نطاق الفلتر التلقائي
            worksheet.AutoFilter.Range = "A1:B4";

            // الحصول على الفلتر التلقائي
            AutoFilter filter = worksheet.AutoFilter;

            // تطبيق الفلتر
            filter.Filter(1, "10");

            // الترتيب باستخدام خاصية Sorter
            filter.Sorter.Sort();

            // احفظ المصنف
            workbook.Save("AutoFilterPropertySorterDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DataSorter](../../datasorter/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


