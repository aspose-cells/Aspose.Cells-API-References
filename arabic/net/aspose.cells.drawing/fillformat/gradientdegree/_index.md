---
title: "FillFormat.GradientDegree"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FillFormat. تُرجع درجة التدرج للملء المحدد. تنطبق فقط على Excel 2007"
type: docs
url: /ar/net/aspose.cells.drawing/fillformat/gradientdegree/
---
## FillFormat.GradientDegree property

يعيد درجة التدرج للملء المحدد. ينطبق فقط على Excel 2007.

```csharp
public double GradientDegree { get; }
```

### ملاحظات

يمكن أن تكون قيمة فقط من 0.0 (داكن) إلى 1.0 (فاتح).

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyGradientDegreeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // تعيين ملء التدرج للسلسلة الأولى
            Aspose.Cells.Drawing.FillFormat fillFormat = chart.NSeries[0].Area.FillFormat;
            fillFormat.SetTwoColorGradient(Color.Red, Color.Blue, Aspose.Cells.Drawing.GradientStyleType.Horizontal, 2);
            
            // عرض درجة التدرج
            Console.WriteLine("Gradient Degree: " + fillFormat.GradientDegree);

            // احفظ المصنف
            workbook.Save("GradientDegreeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


