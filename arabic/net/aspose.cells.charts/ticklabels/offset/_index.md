---
title: "TickLabels.Offset"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TickLabels. تحصل وتحدد مسافة التسميات من محور الفئة. ينطبق هذا فقط على محور الفئة السيني"
type: docs
url: /ar/net/aspose.cells.charts/ticklabels/offset/
---
## TickLabels.Offset property

يحصل أو يعيّن مسافة التسميات من محور الفئة. ينطبق هذا فقط على محور الفئة (x).

```csharp
public int Offset { get; set; }
```

### ملاحظات

المسافة الافتراضية هي 100 بالمئة، والتي تمثل التباعد الافتراضي بين تسميات المحور وخط المحور. يمكن أن تكون القيمة نسبة مئوية صحيحة من 0 إلى 1000، نسبة إلى حجم خط تسمية المحور.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyOffsetDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // إضافة مخطط
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // الوصول إلى محور القيم
            Axis valueAxis = chart.ValueAxis;
            
            // تعيين إزاحة TickLabels
            valueAxis.TickLabels.Offset = 50; // 50% offset from default position

            // احفظ المصنف
            workbook.Save("TickLabelsOffsetDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


