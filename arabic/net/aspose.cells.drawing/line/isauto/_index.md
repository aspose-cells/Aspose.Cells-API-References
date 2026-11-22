---
title: "Line.IsAuto"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Line. تشير إلى ما إذا كان نمط الخط هذا مُعيّن تلقائيًا"
type: docs
url: /ar/net/aspose.cells.drawing/line/isauto/
---
## Line.IsAuto property

يشير إلى ما إذا كان نمط الخط هذا مُعينًا تلقائيًا.

```csharp
public bool IsAuto { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class LinePropertyIsAutoDemo
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
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            try
            {
                // إضافة مخطط خطي
                int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
                Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

                // تعيين نطاق بيانات المخطط
                chart.NSeries.Add("B2:B3", true);
                chart.NSeries.CategoryData = "A2:A3";

                // الوصول إلى خصائص الخط للسلسلة
                Aspose.Cells.Charts.Series series = chart.NSeries[0];
                Line line = series.Border;

                // اعرض قيمة IsAuto الحالية
                Console.WriteLine("Initial IsAuto value: " + line.IsAuto);

                // حدد IsAuto إلى true
                line.IsAuto = true;
                Console.WriteLine("After setting to true, IsAuto value: " + line.IsAuto);

                // حدد IsAuto إلى false
                line.IsAuto = false;
                Console.WriteLine("After setting to false, IsAuto value: " + line.IsAuto);

                // احفظ المصنف
                workbook.Save("IsAutoDemo.xlsx");
                Console.WriteLine("IsAuto property has been demonstrated successfully.");
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

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


