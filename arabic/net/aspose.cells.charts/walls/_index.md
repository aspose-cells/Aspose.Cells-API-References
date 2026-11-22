---
title: "فئة Walls"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Charts.Walls. تغلف الكائن الذي يمثل جدران مخطط ثلاثي الأبعاد"
type: docs
url: /ar/net/aspose.cells.charts/walls/
---
## Walls class

يحتوي على الكائن الذي يمثل جدران مخطط ثلاثي الأبعاد.

```csharp
public class Walls : Floor
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BackgroundColor](../../aspose.cells.drawing/area/backgroundcolor/) { get; set; } | يحصل أو يضبط لون الخلفية للـ [`Area`](../../aspose.cells.drawing/area/). (موروث من [`Area`](../../aspose.cells.drawing/area/).) |
| [Border](../../aspose.cells.charts/floor/border/) { get; set; } | يحصل أو يعيّن الحد [`Line`](../../aspose.cells.drawing/line/).(موروث من [`Floor`](../floor/).) |
| [CenterX](../../aspose.cells.charts/walls/centerx/) { get; } | يحصل على إحداثي x للزاوية اليسرى السفلية لمركز الجدار بوحدات 1/4000 من عرض المخطط بعد استدعاء طريقة Chart.Calculate(). |
| [CenterXPx](../../aspose.cells.charts/walls/centerxpx/) { get; } | يحصل على إحداثي x للزاوية السفلية اليسرى لمركز الجدار بوحدات البكسل بعد استدعاء طريقة Chart.Calculate(). |
| [CenterY](../../aspose.cells.charts/walls/centery/) { get; } | يحصل على إحداثي y للزاوية اليسرى السفلية لمركز الجدار بوحدات 1/4000 من ارتفاع المخطط بعد استدعاء طريقة Chart.Calculate(). |
| [CenterYPx](../../aspose.cells.charts/walls/centerypx/) { get; } | يحصل على إحداثي y للزاوية اليسرى السفلية لمركز الجدار بوحدات البكسل بعد استدعاء طريقة Chart.Calculate(). |
| [Depth](../../aspose.cells.charts/walls/depth/) { get; } | يحصل على العمق من الأمام إلى الخلف بوحدات 1/4000 من عرض المخطط بعد استدعاء طريقة Chart.Calculate(). |
| [DepthPx](../../aspose.cells.charts/walls/depthpx/) { get; } | يحصل على العمق من الأمام إلى الخلف بوحدات البكسل بعد استدعاء طريقة Chart.Calculate(). |
| [FillFormat](../../aspose.cells.drawing/area/fillformat/) { get; } | يمثل كائن [`FillFormat`](../../aspose.cells.drawing/area/fillformat/) الذي يحتوي على خصائص تنسيق التعبئة للمخطط أو الشكل المحدد. (موروث من [`Area`](../../aspose.cells.drawing/area/).) |
| [ForegroundColor](../../aspose.cells.drawing/area/foregroundcolor/) { get; set; } | يحصل أو يضبط لون المقدمة. (موروث من [`Area`](../../aspose.cells.drawing/area/).) |
| [Formatting](../../aspose.cells.drawing/area/formatting/) { get; set; } | يمثل تنسيق المنطقة. (موروث من [`Area`](../../aspose.cells.drawing/area/).) |
| [Height](../../aspose.cells.charts/walls/height/) { get; } | يحصل على الارتفاع من الأعلى إلى الأسفل بوحدات 1/4000 من ارتفاع المخطط بعد استدعاء طريقة Chart.Calculate(). |
| [HeightPx](../../aspose.cells.charts/walls/heightpx/) { get; } | يحصل على الارتفاع من الأعلى إلى الأسفل بوحدات البكسل بعد استدعاء طريقة Chart.Calculate(). |
| [InvertIfNegative](../../aspose.cells.drawing/area/invertifnegative/) { get; set; } | إذا كانت الخاصية true وكانت قيمة نقطة المخطط رقمًا سالبًا، سيتم تبادل لون المقدمة ولون الخلفية. (موروث من [`Area`](../../aspose.cells.drawing/area/).) |
| [Transparency](../../aspose.cells.drawing/area/transparency/) { get; set; } | يرجع أو يضبط درجة شفافية المنطقة كقيمة من 0.0 (معتم) إلى 1.0 (شفاف). (موروث من [`Area`](../../aspose.cells.drawing/area/).) |
| [Width](../../aspose.cells.charts/walls/width/) { get; } | يحصل على العرض من اليسار إلى اليمين بوحدات 1/4000 من عرض المخطط بعد استدعاء طريقة Chart.Calculate(). |
| [WidthPx](../../aspose.cells.charts/walls/widthpx/) { get; } | يحصل على العرض من اليسار إلى اليمين بوحدات البكسل بعد استدعاء طريقة Chart.Calculate(). |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetCubePointCount](../../aspose.cells.charts/walls/getcubepointcount/)() | يحصل على عدد نقاط المكعب بعد استدعاء طريقة Chart.Calculate(). |
| [GetCubePointXPx](../../aspose.cells.charts/walls/getcubepointxpx/)(int) | يحصل على الإحداثي السيني لنقطة القمة لمكعب الجدران بعد استدعاء طريقة Chart.Calculate(). عدد نقاط القمة لمكعب الجدران هو ثمانية |
| [GetCubePointYPx](../../aspose.cells.charts/walls/getcubepointypx/)(int) | يحصل على الإحداثي الصادي لنقطة القمة لمكعب الجدران بعد استدعاء طريقة Chart.Calculate(). عدد نقاط القمة لمكعب الجدران هو ثمانية. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class WallsDemo
    {
        public static void WallsExample()
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

            // أضف مخططًا ثلاثي الأبعاد إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احسب المخطط لتحديث خصائصه
            chart.Calculate();

            // الوصول إلى جدران المخطط ثلاثي الأبعاد
            Walls walls = chart.Walls;

            // تعيين خصائص الجدران
            walls.BackgroundColor = Color.LightBlue;
            walls.ForegroundColor = Color.DarkBlue;
            walls.Formatting = FormattingType.Custom;
            walls.InvertIfNegative = true;
            walls.Transparency = 0.5;

            // الوصول إلى حدود الجدران وتعيين خصائصها
            Line border = walls.Border;
            border.Color = Color.Red;
            border.Style = LineType.Solid;

            // اطبع بعض خصائص الجدران
            Console.WriteLine("CenterX: " + walls.CenterX);
            Console.WriteLine("CenterY: " + walls.CenterY);
            Console.WriteLine("Width: " + walls.Width);
            Console.WriteLine("Depth: " + walls.Depth);
            Console.WriteLine("Height: " + walls.Height);
            Console.WriteLine("CenterXPx: " + walls.CenterXPx);
            Console.WriteLine("CenterYPx: " + walls.CenterYPx);
            Console.WriteLine("WidthPx: " + walls.WidthPx);
            Console.WriteLine("DepthPx: " + walls.DepthPx);
            Console.WriteLine("HeightPx: " + walls.HeightPx);

            // احفظ المصنف
            workbook.Save("WallsExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Floor](../floor/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


