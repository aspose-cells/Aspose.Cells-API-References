---
title: "Chart.DisplayNaAsBlank"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Chart. تشير إلى ما إذا كان يجب عرض N/A كقيمة فارغة"
type: docs
url: /ar/net/aspose.cells.charts/chart/displaynaasblank/
---
## Chart.DisplayNaAsBlank property

يشير إلى ما إذا كان يجب عرض #N/A كقيمة فارغة.

```csharp
public bool DisplayNaAsBlank { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyDisplayNaAsBlankDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات عينة تحتوي على بعض قيم NA
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(double.NaN); // NA value
            worksheet.Cells["B4"].PutValue(30);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // تعيين خاصية DisplayNaAsBlank
            chart.DisplayNaAsBlank = true;

            // احفظ المصنف
            workbook.Save("output.xlsx");

            // تحقق من الخاصية
            Console.WriteLine("DisplayNaAsBlank is set to: " + chart.DisplayNaAsBlank);
        }
    }
}
```

### انظر أيضًا

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


