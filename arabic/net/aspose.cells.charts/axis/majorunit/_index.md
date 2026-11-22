---
title: "Axis.MajorUnit"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Axis. تمثل الوحدات الرئيسية للمحور"
type: docs
url: /ar/net/aspose.cells.charts/axis/majorunit/
---
## Axis.MajorUnit property

يمثل الوحدات الرئيسية للمحور.

```csharp
public double MajorUnit { get; set; }
```

### ملاحظات

يجب أن تكون الوحدات الرئيسية أكبر من الصفر.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMajorUnitDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Category");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Cat " + i);
                worksheet.Cells["B" + (i + 1)].PutValue(i * 10);
            }

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B11", true);
            chart.NSeries.CategoryData = "A2:A11";

            // احصل على محور الفئة
            Axis axis = chart.CategoryAxis;

            // عرض الوحدة الرئيسية الأولية
            Console.WriteLine("Initial Major Unit: " + axis.MajorUnit);

            // تعيين وحدة رئيسية جديدة
            axis.MajorUnit = 3;
            Console.WriteLine("Modified Major Unit: " + axis.MajorUnit);

            // احفظ المصنف
            workbook.Save("AxisMajorUnitDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


