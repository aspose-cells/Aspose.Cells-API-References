---
title: "Area.Transparency"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Area. تُعيد أو تعين درجة الشفافية للمنطقة كقيمة من 0.0 غير شفاف إلى 1.0 شفاف"
type: docs
url: /ar/net/aspose.cells.drawing/area/transparency/
---
## Area.Transparency property

يعيد أو يضبط درجة شفافية المنطقة كقيمة من 0.0 (معتم) إلى 1.0 (شفاف).

```csharp
public double Transparency { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AreaPropertyTransparencyDemo
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

            // الوصول إلى السلسلة الأولى
            Aspose.Cells.Charts.Series series = chart.NSeries[0];

            // عرض خاصية Transparency
            Console.WriteLine("Initial area transparency: " + series.Area.Transparency);
            Console.WriteLine("Initial border transparency: " + series.Border.Transparency);

            // تعديل قيم الشفافية
            series.Area.Transparency = 0.5; // 50% transparent
            series.Border.Transparency = 0.2; // 20% transparent

            Console.WriteLine("Modified area transparency: " + series.Area.Transparency);
            Console.WriteLine("Modified border transparency: " + series.Border.Transparency);

            // احفظ المصنف
            workbook.Save("AreaPropertyTransparencyDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


