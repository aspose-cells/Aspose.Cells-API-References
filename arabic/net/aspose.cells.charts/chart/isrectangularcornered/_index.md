---
title: "Chart.IsRectangularCornered"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Chart. يحصل أو يضبط قيمة تشير إلى ما إذا كانت مساحة المخطط ذات زوايا مستطيلة. القيمة الافتراضية هي true"
type: docs
url: /ar/net/aspose.cells.charts/chart/isrectangularcornered/
---
## Chart.IsRectangularCornered property

يحصل أو يعيّن قيمة تشير إلى ما إذا كانت مساحة المخطط ذات زوايا مستطيلة. القيمة الافتراضية هي true.

```csharp
public bool IsRectangularCornered { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyIsRectangularCorneredDemo
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

            // أضف مخطط عمودي
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // عرض خاصية IsRectangularCornered
            Console.WriteLine("Default IsRectangularCornered: " + chart.IsRectangularCornered);
            
            // اضبطه على true لجعل زوايا المخطط مستطيلة
            chart.IsRectangularCornered = true;
            Console.WriteLine("After setting IsRectangularCornered to true: " + chart.IsRectangularCornered);

            // احفظ المصنف
            workbook.Save("ChartPropertyIsRectangularCorneredDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


