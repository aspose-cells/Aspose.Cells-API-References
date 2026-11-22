---
title: "تعداد SparklineType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Charts.SparklineType enum. يمثل أنواع sparkline"
type: docs
url: /ar/net/aspose.cells.charts/sparklinetype/
---
## SparklineType enumeration

يمثل أنواع الـ sparkline.

```csharp
public enum SparklineType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Line | `0` | خط sparkline. |
| Column | `1` | مخطط شراري للعمود. |
| Stacked | `2` | يمثل مخططًا شراريًا للفوز/الخسارة. |
| WinLoss | `2` | يمثل مخططًا شراريًا للفوز/الخسارة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class SparklineTypeDemo
    {
        public static void SparklineTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات إلى ورقة العمل
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);

            // حدد CellArea للمخطط الخطي.
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // أضف مجموعة مخطط خطي إلى ورقة العمل.
            int idx = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = worksheet.SparklineGroups[idx];

            // أضف مخططات خطية إلى المجموعة.
            group.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);

            // تخصيص مجموعة المخططات الشرارية
            CellsColor clr = workbook.CreateCellsColor();
            clr.Color = Color.Orange;
            group.SeriesColor = clr;

            // اجعل النقاط العالية ملونة بالأخضر والنقاط المنخفضة ملونة بالأحمر
            group.ShowHighPoint = true;
            group.ShowLowPoint = true;
            group.HighPointColor.Color = Color.Green;
            group.LowPointColor.Color = Color.Red;

            // حدد وزن الخط.
            group.LineWeight = 1.0;

            // احفظ المصنف
            workbook.Save("SparklineTypeExample.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


