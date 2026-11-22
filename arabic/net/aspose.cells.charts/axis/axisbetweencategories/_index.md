---
title: "Axis.AxisBetweenCategories"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Axis. تمثل ما إذا كان محور القيمة يعبر محور الفئة بين الفئات"
type: docs
url: /ar/net/aspose.cells.charts/axis/axisbetweencategories/
---
## Axis.AxisBetweenCategories property

يمثل ما إذا كان محور القيمة يعبر محور الفئة بين الفئات.

```csharp
public bool AxisBetweenCategories { get; set; }
```

### ملاحظات

تنطبق هذه الخاصية فقط على محاور الفئات، ولا تنطبق على المخططات ثلاثية الأبعاد.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AxisPropertyAxisBetweenCategoriesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى وإضافة بيانات نموذجية
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Categories");
            worksheet.Cells["B1"].PutValue("Values");
            
            for (int i = 1; i <= 5; i++)
            {
                worksheet.Cells[$"A{i+1}"].PutValue($"Category {i}");
                worksheet.Cells[$"B{i+1}"].PutValue(i * 10);
            }

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين بيانات المخطط
            chart.NSeries.Add("B2:B6", true);
            chart.NSeries.CategoryData = "A2:A6";

            // قم بتكوين محور الفئة
            Axis categoryAxis = chart.CategoryAxis;
            categoryAxis.AxisBetweenCategories = false; // Core property demonstration
            categoryAxis.TickLabels.RotationAngle = 45;

            // احفظ المصنف
            workbook.Save("AxisBetweenCategoriesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


