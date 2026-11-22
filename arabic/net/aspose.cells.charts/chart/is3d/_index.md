---
title: "Chart.Is3D"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Chart. تشير إلى ما إذا كان المخطط مخططًا ثلاثي الأبعاد"
type: docs
url: /ar/net/aspose.cells.charts/chart/is3d/
---
## Chart.Is3D property

يشير إلى ما إذا كان المخطط مخططًا ثلاثي الأبعاد.

```csharp
public bool Is3D { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPropertyIs3DDemo
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

            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(1500);
            worksheet.Cells["B4"].PutValue(1800);
            worksheet.Cells["B5"].PutValue(2100);

            // أضف مخطط عمودي
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 6, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // حدد نطاق البيانات للمخطط
            chart.SetChartDataRange("A1:B5", true);

            // عرض قيمة Is3D الحالية
            Console.WriteLine("Current Is3D value: " + chart.Is3D);

            // إنشاء نسخة ثلاثية الأبعاد من المخطط
            int chart3DIndex = worksheet.Charts.Add(ChartType.Column3D, 6, 12, 20, 22);
            Chart chart3D = worksheet.Charts[chart3DIndex];
            chart3D.SetChartDataRange("A1:B5", true);

            // عرض قيمة Is3D للمخطط ثلاثي الأبعاد
            Console.WriteLine("3D Chart Is3D value: " + chart3D.Is3D);

            // احفظ المصنف
            workbook.Save("ChartPropertyIs3DDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


