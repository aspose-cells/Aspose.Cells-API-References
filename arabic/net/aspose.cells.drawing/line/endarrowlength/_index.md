---
title: "Line.EndArrowLength"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Line. تحدد طول رأس السهم لنهاية الخط"
type: docs
url: /ar/net/aspose.cells.drawing/line/endarrowlength/
---
## Line.EndArrowLength property

يحدد طول رأس السهم لنهاية الخط.

```csharp
public MsoArrowheadLength EndArrowLength { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class LinePropertyEndArrowLengthDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إنشاء ورقة عمل نموذجية
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات لجعل المثال ذو معنى
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["B1"].PutValue("Values");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(40);

            try
            {
                // أضف مخططًا لتوضيح خصائص الخط
                int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 15, 5);
                Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("A1:B3", true);

                // احصل على خصائص الخط من حد سلسلة المخطط
                Line line = chart.NSeries[0].Border;

                // حدد نوع رأس السهم لعرض EndArrowLength
                line.EndType = MsoArrowheadStyle.Arrow;

                // اعرض قيمة EndArrowLength الحالية
                Console.WriteLine("Current EndArrowLength: " + line.EndArrowLength);

                // حدد قيمة EndArrowLength جديدة
                line.EndArrowLength = MsoArrowheadLength.Long;
                Console.WriteLine("Updated EndArrowLength: " + line.EndArrowLength);

                // احفظ المصنف
                workbook.Save("EndArrowLengthDemo.xlsx");
                Console.WriteLine("EndArrowLength property demonstrated successfully.");
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


