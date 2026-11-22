---
title: "ChartFrame.HeightPixel"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartFrame. تحصل أو تعين ارتفاع الإطار بوحدات البكسل"
type: docs
url: /ar/net/aspose.cells.charts/chartframe/heightpixel/
---
## ChartFrame.HeightPixel property

يحصل على أو يضبط ارتفاع الإطار بوحدات البكسل.

```csharp
public virtual int HeightPixel { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyHeightPixelDemo
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
            
            // الوصول إلى عنوان المخطط (الذي هو ChartFrame)
            ChartFrame chartTitle = chart.Title;
            
            // عرض الارتفاع الحالي بالبكسل
            Console.WriteLine("Current title height: " + chartTitle.HeightPixel + " pixels");
            
            // تعيين ارتفاع جديد للعنوان
            chartTitle.HeightPixel = 40;
            Console.WriteLine("New title height: " + chartTitle.HeightPixel + " pixels");
            
            // الوصول إلى وسيلة الإيضاح (ChartFrame آخر)
            ChartFrame legend = chart.Legend;
            
            // عرض وتعديل ارتفاع وسيلة الإيضاح
            Console.WriteLine("Current legend height: " + legend.HeightPixel + " pixels");
            legend.HeightPixel = 60;
            Console.WriteLine("New legend height: " + legend.HeightPixel + " pixels");
            
            // احفظ المصنف
            workbook.Save("ChartFrameHeightPixelDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


