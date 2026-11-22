---
title: "Title.Y"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Title. تحصل أو تعين إحداثي y للزاوية العلوية اليسرى بوحدات 1/4000 من مساحة المخطط"
type: docs
url: /ar/net/aspose.cells.charts/title/y/
---
## Title.Y property

تحصل أو تعين إحداثي y للزاوية العلوية اليسرى بوحدات 1/4000 من مساحة المخطط.

```csharp
[Obsolete("Use Title.YRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Y { get; set; }
```

### ملاحظات

ملاحظة: هذا العضو أصبح الآن مهجورًا. يرجى استخدام خاصية Title.YRatioToChart بدلاً من ذلك. Y = YRatioToChart * 4000; سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ فبراير 2025. تقدم Aspose اعتذارًا عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TitlePropertyYDemo
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
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // تعيين عنوان المخطط
            chart.Title.Text = "Sample Chart";
            chart.Title.Y = 1000; // Demonstrating Y property - position in 1/4000 units
            
            // احسب المخطط لضمان تحديث التخطيط
            chart.Calculate();

            // أضف شكلًا محاذيًا لموضع Y للعنوان
            Shape shape = chart.Shapes.AddShapeInChart(MsoDrawingType.Rectangle, PlacementType.Move,
                2000, 
                chart.Title.Y, // Using the title's Y property
                3000, 
                chart.Title.Y + 500);
            shape.Fill.SolidFill.Color = Color.Blue;

            // احفظ المصنف
            workbook.Save("TitlePropertyYDemo_Output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


