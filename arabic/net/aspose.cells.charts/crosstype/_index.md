---
title: "تعداد CrossType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Charts.CrossType enum. يمثل نوع تقاطع المحور"
type: docs
url: /ar/net/aspose.cells.charts/crosstype/
---
## CrossType enumeration

يمثل نوع تقاطع المحور.

```csharp
public enum CrossType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Automatic | `0` | Microsoft Excel يحدد نقطة تقاطع المحور. |
| Maximum | `1` | المحور يتقاطع عند القيمة القصوى. |
| Minimum | `2` | المحور يقطع عند القيمة الدنيا. |
| Custom | `3` | المحور يقطع عند القيمة المخصصة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class CrossTypeDemo
    {
        public static void CrossTypeExample()
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
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            // الوصول إلى نسخة المخطط المضاف حديثًا
            Chart chart = worksheet.Charts[chartIndex];
            // إضافة NSeries (مصدر بيانات المخطط) إلى المخطط من الخلية "A1" إلى "B3"
            chart.NSeries.Add("A1:B3", true);

            // حدد القيمة القصوى لمحور القيم
            chart.ValueAxis.MaxValue = 200;
            // حدد القيمة الدنيا لمحور القيم
            chart.ValueAxis.MinValue = 0;
            // حدد الوحدة الرئيسية
            chart.ValueAxis.MajorUnit = 25;

            // محور الفئة (X) يقطع عند القيمة القصوى
            chart.ValueAxis.CrossType = CrossType.Maximum;

            // حدد عدد الفئات أو السلاسل بين تسميات علامات الفواصل
            chart.CategoryAxis.TickLabelSpacing = 2;

            // حفظ ملف Excel
            workbook.Save("CrossTypeExample.xlsx");
            workbook.Save("CrossTypeExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


