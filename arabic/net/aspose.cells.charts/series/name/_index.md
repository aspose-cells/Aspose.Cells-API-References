---
title: "Series.Name"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Series. تحصل أو تعين اسم سلسلة البيانات"
type: docs
url: /ar/net/aspose.cells.charts/series/name/
---
## Series.Name property

يحصل على أو يضبط اسم سلسلة البيانات.

```csharp
public string Name { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Series Name");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["C2"].PutValue(30);
            
            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // إضافة سلسلة إلى المخطط
            chart.NSeries.Add("A2:C2", true);
            
            // عرض استخدام خاصية Name
            // 1. اسم مرجعي إلى خلية
            chart.NSeries[0].Name = "=A1";
            
            // 2. تعيين سلسلة كاسم
            chart.NSeries[0].Name = "First Series";
            
            // احفظ المصنف
            workbook.Save("SeriesPropertyNameDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


