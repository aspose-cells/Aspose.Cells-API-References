---
title: "Line.IsAutomaticColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Line. تشير إلى ما إذا كان لون الخط مُعيّن تلقائيًا"
type: docs
url: /ar/net/aspose.cells.drawing/line/isautomaticcolor/
---
## Line.IsAutomaticColor property

يشير إلى ما إذا كان لون الخط مُعينًا تلقائيًا.

```csharp
public bool IsAutomaticColor { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class LinePropertyIsAutomaticColorDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية لمخطط
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

                // اقرأ واعرض قيمة خاصية IsAutomaticColor
                Console.WriteLine("IsAutomaticColor value: " + seriesLine.IsAutomaticColor);

                // احفظ المصنف
                workbook.Save("IsAutomaticColorDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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


