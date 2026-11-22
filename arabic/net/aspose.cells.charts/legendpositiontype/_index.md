---
title: "تعداد LegendPositionType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Charts.LegendPositionType enum. يعدد أنواع مواضع وسيلة الإيضاح"
type: docs
url: /ar/net/aspose.cells.charts/legendpositiontype/
---
## LegendPositionType enumeration

يسرد أنواع موضع وسيلة الإيضاح.

```csharp
public enum LegendPositionType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Bottom | `0` | يعرض وسيلة الإيضاح في أسفل منطقة رسم المخطط. |
| Corner | `1` | يعرض وسيلة الإيضاح في زاوية منطقة رسم المخطط. |
| Left | `4` | يعرض وسيلة الإيضاح إلى يسار منطقة رسم المخطط. |
| NotDocked | `7` | يشير إلى أن وسيلة الإيضاح غير مثبتة. |
| Right | `3` | يعرض وسيلة الإيضاح إلى يمين منطقة رسم المخطط. |
| Top | `2` | يعرض وسيلة الإيضاح في أعلى منطقة رسم المخطط. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LegendPositionTypeDemo
    {
        public static void LegendPositionTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            Cells cells = sheet.Cells;
            cells[0, 1].PutValue("Income");
            cells[1, 0].PutValue("Company A");
            cells[2, 0].PutValue("Company B");
            cells[3, 0].PutValue("Company C");
            cells[1, 1].PutValue(10000);
            cells[2, 1].PutValue(20000);
            cells[3, 1].PutValue(30000);

            // إضافة مخطط عمودي إلى ورقة العمل
            int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
            Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // الوصول إلى وسيلة الإيضاح للمخطط
            Legend legend = chart.Legend;

            // ضبط موضع وسيلة الإيضاح إلى يسار المخطط
            legend.Position = LegendPositionType.Left;

            // ضبط خصائص إضافية لوسيلة الإيضاح
            legend.Y = 1500;
            legend.Width = 50;
            legend.Height = 50;

            // احفظ المصنف
            workbook.Save("LegendPositionTypeExample.xlsx");
            workbook.Save("LegendPositionTypeExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


