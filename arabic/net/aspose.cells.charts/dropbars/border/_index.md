---
title: "DropBars.Border"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DropBars. تحصل على خط الحدود"
type: docs
url: /ar/net/aspose.cells.charts/dropbars/border/
---
## DropBars.Border property

تحصل على الخط الحد [`Line`](../../../aspose.cells.drawing/line/).

```csharp
public Line Border { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class DropBarsPropertyBorderDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // إضافة مخطط خطي
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // إضافة سلسلة بيانات إلى المخطط.
            chart.NSeries.Add("A1:B3", true);

            // تمكين أشرطة الصعود/الهبوط
            chart.NSeries[0].HasUpDownBars = true;

            try
            {
                // الوصول إلى كائنات DropBars
                DropBars upBars = chart.NSeries[0].UpBars;
                DropBars downBars = chart.NSeries[0].DownBars;

                // عرض خصائص الحدود الحالية (وصول للقراءة فقط)
                Console.WriteLine("Up Bars Border Color: " + upBars.Border.Color);
                Console.WriteLine("Up Bars Border Style: " + upBars.Border.Style);
                Console.WriteLine("Up Bars Border Weight: " + upBars.Border.WeightPt);
                Console.WriteLine("Up Bars Border Visibility: " + upBars.Border.IsVisible);

                Console.WriteLine("\nDown Bars Border Color: " + downBars.Border.Color);
                Console.WriteLine("Down Bars Border Style: " + downBars.Border.Style);
                Console.WriteLine("Down Bars Border Weight: " + downBars.Border.WeightPt);
                Console.WriteLine("Down Bars Border Visibility: " + downBars.Border.IsVisible);

                // تعديل خصائص الحدود (لأن Line ليست للقراءة فقط)
                upBars.Border.Color = Color.Blue;
                upBars.Border.Style = LineType.Solid;
                upBars.Border.WeightPt = 2.0;
                upBars.Border.IsVisible = true;

                downBars.Border.Color = Color.Red;
                downBars.Border.Style = LineType.Dash;
                downBars.Border.WeightPt = 1.5;
                downBars.Border.IsVisible = true;

                // احفظ المصنف
                workbook.Save("DropBarsBorderDemo.xlsx");
                Console.WriteLine("\nBorder properties have been demonstrated and saved to file.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Line](../../../aspose.cells.drawing/line/)
* class [DropBars](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


