---
title: "Chart.PrintSize"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Chart. تحصل على حجم المخطط المطبوع وتضبطه"
type: docs
url: /ar/net/aspose.cells.charts/chart/printsize/
---
## Chart.PrintSize property

يحصل على حجم المخطط المطبوع ويضبطه.

```csharp
public PrintSizeType PrintSize { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPrintSizeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // تكوين إعدادات الطباعة
            chart.PrintSize = PrintSizeType.Full;
            chart.SizeWithWindow = false;
            chart.AutoScaling = false;

            // احفظ المصنف
            workbook.Save("ChartPrintSizeDemo.pdf", SaveFormat.Pdf);
        }
    }
}
```

### انظر أيضًا

* enum [PrintSizeType](../../../aspose.cells/printsizetype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


