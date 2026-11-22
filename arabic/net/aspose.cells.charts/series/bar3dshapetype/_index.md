---
title: "Series.Bar3DShapeType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Series. يحصل أو يضبط نوع الشكل ثلاثي الأبعاد المستخدم مع مخطط الشريط أو العمود ثلاثي الأبعاد"
type: docs
url: /ar/net/aspose.cells.charts/series/bar3dshapetype/
---
## Series.Bar3DShapeType property

يحصل أو يحدد نوع الشكل ثلاثي الأبعاد المستخدم مع مخطط الأعمدة أو المخطط العمودي ثلاثي الأبعاد.

```csharp
public Bar3DShapeType Bar3DShapeType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyBar3DShapeTypeDemo
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

            // أضف مخطط شريط ثلاثي الأبعاد
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // حدد نوع شكل الشريط إلى أسطوانة
            chart.NSeries[0].Bar3DShapeType = Bar3DShapeType.Cylinder;

            // احفظ المصنف
            workbook.Save("Bar3DShapeTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* enum [Bar3DShapeType](../../bar3dshapetype/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


