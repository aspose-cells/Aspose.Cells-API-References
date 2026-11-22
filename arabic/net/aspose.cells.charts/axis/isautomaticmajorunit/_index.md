---
title: "Axis.IsAutomaticMajorUnit"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Axis. تشير إلى ما إذا كانت الوحدة الرئيسية للمحور تُعيّن تلقائيًا"
type: docs
url: /ar/net/aspose.cells.charts/axis/isautomaticmajorunit/
---
## Axis.IsAutomaticMajorUnit property

يشير إلى ما إذا كانت الوحدة الرئيسية للمحور تُعيّن تلقائيًا.

```csharp
public bool IsAutomaticMajorUnit { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsAutomaticMajorUnitDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // تحقق وعرض حالة الوحدة الرئيسية التلقائية
            Console.WriteLine("IsAutomaticMajorUnit (default): " + chart.ValueAxis.IsAutomaticMajorUnit);
            
            // تعطيل الوحدة الرئيسية التلقائية وتعيين قيمة مخصصة
            chart.ValueAxis.IsAutomaticMajorUnit = false;
            chart.ValueAxis.MajorUnit = 5;
            Console.WriteLine("IsAutomaticMajorUnit (after change): " + chart.ValueAxis.IsAutomaticMajorUnit);
        }
    }
}
```

### انظر أيضًا

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


