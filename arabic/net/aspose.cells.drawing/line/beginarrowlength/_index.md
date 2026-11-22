---
title: "Line.BeginArrowLength"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية الخط. تحدد طول رأس السهم لبداية الخط"
type: docs
url: /ar/net/aspose.cells.drawing/line/beginarrowlength/
---
## Line.BeginArrowLength property

يحدد طول رأس السهم لبداية الخط.

```csharp
public MsoArrowheadLength BeginArrowLength { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class LinePropertyBeginArrowLengthDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إعداد بيانات بسيطة للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            try
            {
                // إضافة مخطط خطي
                int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
                Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("B2:B3", true);
                chart.NSeries.CategoryData = "A2:A3";

                // الوصول إلى الخط (الحد) للسلسلة الأولى
                Line seriesLine = chart.NSeries[0].Border;

                // ضبط BeginArrowLength إلى Long
                seriesLine.BeginArrowLength = MsoArrowheadLength.Long;

                // قراءة وعرض القيمة الحالية لـ BeginArrowLength
                Console.WriteLine("BeginArrowLength value: " + seriesLine.BeginArrowLength);

                // احفظ المصنف (اختياري، فقط لإكمال العرض التجريبي)
                workbook.Save("BeginArrowLengthDemo.xlsx");
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

* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


