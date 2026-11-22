---
title: "ChartFrame.YPixel"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartFrame. تحصل أو تعين إحداثي y للزاوية العلوية اليسرى بوحدات البكسل"
type: docs
url: /ar/net/aspose.cells.charts/chartframe/ypixel/
---
## ChartFrame.YPixel property

يحصل على أو يضبط إحداثي y للزاوية العليا اليسرى بوحدات البكسل.

```csharp
public virtual int YPixel { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyYPixelDemo
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

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 5, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // الوصول إلى عنوان المخطط (الذي يرث من ChartFrame)
            chart.Title.Text = "Sample Chart";
            ChartFrame chartFrame = chart.Title;

            // عرض قيمة YPixel الحالية
            Console.WriteLine("Current YPixel value: " + chartFrame.YPixel);

            // غيّر موضع YPixel لعنوان المخطط
            chartFrame.YPixel = 50;
            Console.WriteLine("New YPixel value: " + chartFrame.YPixel);

            // احفظ المصنف
            workbook.Save("ChartFrameYPixelDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


