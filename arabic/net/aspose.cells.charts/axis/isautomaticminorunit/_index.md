---
title: "Axis.IsAutomaticMinorUnit"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية المحور. تشير إلى ما إذا كانت الوحدة الصغرى للمحور تُعيّن تلقائيًا"
type: docs
url: /ar/net/aspose.cells.charts/axis/isautomaticminorunit/
---
## Axis.IsAutomaticMinorUnit property

يشير إلى ما إذا كانت الوحدة الثانوية للمحور تُعيّن تلقائيًا.

```csharp
public bool IsAutomaticMinorUnit { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsAutomaticMinorUnitDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // احصل على محور القيمة
            Axis valueAxis = chart.ValueAxis;

            // عرض خاصية IsAutomaticMinorUnit
            Console.WriteLine("Initial IsAutomaticMinorUnit: " + valueAxis.IsAutomaticMinorUnit);
            
            // تعيين الوحدة الصغرى يدويًا
            valueAxis.IsAutomaticMinorUnit = false;
            valueAxis.MinorUnit = 2;
            Console.WriteLine("After setting manually - IsAutomaticMinorUnit: " + valueAxis.IsAutomaticMinorUnit);
            Console.WriteLine("MinorUnit: " + valueAxis.MinorUnit);

            // إعادة الضبط إلى الوضع التلقائي
            valueAxis.IsAutomaticMinorUnit = true;
            Console.WriteLine("After setting automatic - IsAutomaticMinorUnit: " + valueAxis.IsAutomaticMinorUnit);

            // احفظ المصنف
            workbook.Save("AxisPropertyIsAutomaticMinorUnitDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


