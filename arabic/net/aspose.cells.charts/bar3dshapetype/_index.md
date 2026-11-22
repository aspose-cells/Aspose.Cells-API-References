---
title: "التعداد Bar3DShapeType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Charts.Bar3DShapeType. يمثل الشكل المستخدم مع مخطط العمود ثلاثي الأبعاد"
type: docs
url: /ar/net/aspose.cells.charts/bar3dshapetype/
---
## Bar3DShapeType enumeration

يمثل الشكل المستخدم مع مخطط العمود أو الشريط ثلاثي الأبعاد.

```csharp
public enum Bar3DShapeType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Box | `0` | صندوق |
| PyramidToPoint | `1` | PyramidToPoint |
| PyramidToMax | `2` | PyramidToMax |
| Cylinder | `3` | Cylinder |
| ConeToPoint | `4` | ConeToPoint |
| ConeToMax | `5` | ConeToMax |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class Bar3DShapeTypeDemo
    {
        public static void Bar3DShapeTypeExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();
            // إضافة ورقة عمل جديدة إلى كائن Excel
            int sheetIndex = workbook.Worksheets.Add();
            // الحصول على مرجع ورقة العمل التي تم إضافتها حديثًا بتمرير sheet index
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // إضافة قيم عينة إلى الخلايا
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column3DClustered, 5, 0, 15, 5);
            // الوصول إلى نسخة المخطط المضاف حديثًا
            Chart chart = worksheet.Charts[chartIndex];
            // إضافة NSeries (مصدر بيانات المخطط) إلى المخطط من الخلية "A1" إلى "B4"
            int seriesIndex = chart.NSeries.Add("A1:B4", true);
            // تعيين مصدر البيانات لبيانات الفئة في NSeries
            chart.NSeries.CategoryData = "C1:C4";
            Series series = chart.NSeries[seriesIndex];
            // ضبط قيم السلسلة
            series.Values = "=B1:B4";

            // ضبط نوع الشكل ثلاثي الأبعاد للسلسلة
            series.Bar3DShapeType = Bar3DShapeType.Cylinder;

            // حفظ ملف Excel
            workbook.Save("Bar3DShapeTypeExample.xlsx");
            workbook.Save("Bar3DShapeTypeExample.pdf");

            // ضبط نوع الشكل ثلاثي الأبعاد للسلسلة
            series.Bar3DShapeType = Bar3DShapeType.ConeToMax;

            // حفظ ملف Excel
            workbook.Save("Bar3DShapeTypeExample2.xlsx");
            workbook.Save("Bar3DShapeTypeExample2.pdf");
            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


