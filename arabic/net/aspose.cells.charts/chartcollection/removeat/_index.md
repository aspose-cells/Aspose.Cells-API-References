---
title: "ChartCollection.RemoveAt"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ChartCollection. إزالة مخطط عند الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells.charts/chartcollection/removeat/
---
## ChartCollection.RemoveAt method

إزالة مخطط عند الفهرس المحدد.

```csharp
public void RemoveAt(int index)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | Int32 | فهرس المخطط. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(20);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // عرض عدد المخططات الأولي
            Console.WriteLine("Initial chart count: " + sheet.Charts.Count);

            // إزالة المخطط عند الفهرس 0
            sheet.Charts.RemoveAt(0);

            // عرض عدد المخططات بعد الإزالة
            Console.WriteLine("Chart count after removal: " + sheet.Charts.Count);
        }
    }
}
```

### انظر أيضًا

* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


