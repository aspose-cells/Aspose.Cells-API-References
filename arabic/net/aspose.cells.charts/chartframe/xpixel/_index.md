---
title: "ChartFrame.XPixel"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartFrame. تحصل أو تعين إحداثي x للزاوية العليا اليسرى بوحدات Pixel"
type: docs
url: /ar/net/aspose.cells.charts/chartframe/xpixel/
---
## ChartFrame.XPixel property

يحصل على أو يضبط إحداثي x للزاوية العليا اليسرى بوحدات البكسل.

```csharp
public virtual int XPixel { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyXPixelDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // الوصول إلى عنوان المخطط (الذي يرث من ChartFrame)
            chart.Title.Text = "Sample Chart";
            
            // عرض موضع XPixel الحالي للعنوان
            Console.WriteLine("Current Title XPixel position: " + chart.Title.XPixel);
            
            // تحريك العنوان أفقيًا عن طريق تغيير XPixel
            chart.Title.XPixel = 200;
            
            // عرض موضع XPixel الجديد
            Console.WriteLine("New Title XPixel position: " + chart.Title.XPixel);
            
            // احفظ المصنف
            workbook.Save("ChartFrameXPixelDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


