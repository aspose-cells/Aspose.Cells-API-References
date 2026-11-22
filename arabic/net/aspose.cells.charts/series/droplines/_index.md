---
title: "Series.DropLines"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Series. تُرجع كائن Line الذي يمثل خطوط السقوط لسلسلة في المخطط الخطي أو مخطط المنطقة. ينطبق فقط على المخططات الخطية أو مخططات المنطقة"
type: docs
url: /ar/net/aspose.cells.charts/series/droplines/
---
## Series.DropLines property

تُرجع كائن [`Line`](../../../aspose.cells.drawing/line/) الذي يمثل خطوط السقوط لسلسلة في المخطط الخطي أو مخطط المنطقة. ينطبق فقط على المخططات الخطية أو مخططات المنطقة.

```csharp
public Line DropLines { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class SeriesPropertyDropLinesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["A5"].PutValue("Q4");

            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(120);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(180);
            worksheet.Cells["B5"].PutValue(210);

            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["C2"].PutValue(90);
            worksheet.Cells["C3"].PutValue(130);
            worksheet.Cells["C4"].PutValue(160);
            worksheet.Cells["C5"].PutValue(190);

            // إضافة مخطط خطي
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 6, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.Add("C2:C5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // تمكين خطوط السقوط للمخطط
            chart.NSeries[0].HasDropLines = true;
            chart.NSeries[1].HasDropLines = true;

            // الوصول إلى خطوط السقوط للسلسلة الأولى
            Line dropLines = chart.NSeries[0].DropLines;

            // عرض خصائص خطوط السقوط الحالية
            Console.WriteLine("Drop line color: " + dropLines.Color);
            Console.WriteLine("Drop line style: " + dropLines.Style);
            Console.WriteLine("Drop line weight: " + dropLines.Weight);

            // تعديل خصائص خطوط السقوط
            dropLines.Color = System.Drawing.Color.Red;
            dropLines.Style = LineType.Solid;
            dropLines.Weight = WeightType.MediumLine;
            dropLines.DashType = MsoLineDashStyle.Solid;
            dropLines.IsVisible = true;

            // احفظ المصنف
            workbook.Save("SeriesPropertyDropLinesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Line](../../../aspose.cells.drawing/line/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


