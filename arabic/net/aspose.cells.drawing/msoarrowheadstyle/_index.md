---
title: "تعداد MsoArrowheadStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Drawing.MsoArrowheadStyle enum. يعدد نوع نهاية الخط لحدود الشكل"
type: docs
url: /ar/net/aspose.cells.drawing/msoarrowheadstyle/
---
## MsoArrowheadStyle enumeration

يسرد نوع نهاية الخط لحد الشكل.

```csharp
public enum MsoArrowheadStyle
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | لا نوع لنهاية الخط. |
| Arrow | `1` | نوع نهاية الخط السهم. |
| ArrowStealth | `2` | نوع نهاية الخط السهم المخفي. |
| ArrowDiamond | `3` | نوع نهاية الخط سهم الماس. |
| ArrowOval | `4` | نوع نهاية الخط سهم بيضاوي. |
| ArrowOpen | `5` | نوع نهاية الخط سهم مفتوح. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassMsoArrowheadStyleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكل خط
            LineShape lineShape = worksheet.Shapes.AddLine(5, 5, 10, 10, 100, 100);

            // حدد خصائص الخط
            MsoLineFormat lineFormat = lineShape.LineFormat;
            lineFormat.ForeColor = System.Drawing.Color.Black;
            lineFormat.DashStyle = MsoLineDashStyle.DashDot;
            lineFormat.Weight = 0.75;

            // حدد أنماط رأس السهم
            lineShape.Line.BeginArrowheadStyle = MsoArrowheadStyle.ArrowStealth;
            lineShape.Line.EndArrowheadStyle = MsoArrowheadStyle.Arrow;
            lineShape.Line.BeginArrowheadLength = MsoArrowheadLength.Medium;
            lineShape.Line.EndArrowheadLength = MsoArrowheadLength.Medium;

            // احفظ المصنف
            workbook.Save("MsoArrowheadStyleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


