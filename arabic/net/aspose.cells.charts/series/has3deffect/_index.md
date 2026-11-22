---
title: "Series.Has3DEffect"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية السلسلة. صحيحة إذا كان للمسلسل مظهر ثلاثي الأبعاد"
type: docs
url: /ar/net/aspose.cells.charts/series/has3deffect/
---
## Series.Has3DEffect property

صحيح إذا كان للسلسلة مظهر ثلاثي الأبعاد.

```csharp
public bool Has3DEffect { get; set; }
```

### ملاحظات

ينطبق فقط على مخططات الفقاعات أو Bubble3D.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyHas3DEffectDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Q3");

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // إضافة سلسلة
            int seriesIndex = chart.NSeries.Add("A1:B3", true);
            chart.NSeries.CategoryData = "C1:C3";
            
            // الحصول على السلسلة وتعيين تأثير ثلاثي الأبعاد
            Series series = chart.NSeries[seriesIndex];
            series.Has3DEffect = true;
            series.Bar3DShapeType = Bar3DShapeType.Cylinder;

            // احفظ المصنف
            workbook.Save("Series3DEffectDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


