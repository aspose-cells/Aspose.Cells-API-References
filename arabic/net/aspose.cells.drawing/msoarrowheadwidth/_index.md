---
title: "التعداد MsoArrowheadWidth"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Drawing.MsoArrowheadWidth. يعدد عرض نهاية الخط لحدود الشكل"
type: docs
url: /ar/net/aspose.cells.drawing/msoarrowheadwidth/
---
## MsoArrowheadWidth enumeration

يسرد عرض نهاية الخط لحد الشكل.

```csharp
public enum MsoArrowheadWidth
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Narrow | `0` | عرض نهاية الخط قصير. |
| Medium | `1` | عرض نهاية الخط متوسط. |
| Wide | `2` | عرض نهاية الخط واسع. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class MsoArrowheadWidthDemo
    {
        public static void MsoArrowheadWidthExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.SetChartDataRange("A1:B4", true);

            // إنشاء شكل خط للمخطط
            Line line = chart.Line;

            // تعيين أنماط رؤوس السهام والعروض
            line.BeginType = MsoArrowheadStyle.Arrow;
            line.BeginArrowWidth = MsoArrowheadWidth.Wide;
            line.EndType = MsoArrowheadStyle.Arrow;
            line.EndArrowWidth = MsoArrowheadWidth.Narrow;

            // إخراج أنماط رؤوس السهام والعروض
            Console.WriteLine("Begin Arrowhead Width: " + line.BeginArrowWidth);
            Console.WriteLine("End Arrowhead Width: " + line.EndArrowWidth);

            // احفظ المصنف
            workbook.Save("MsoArrowheadWidthExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


