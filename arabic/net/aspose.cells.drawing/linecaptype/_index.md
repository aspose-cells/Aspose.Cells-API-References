---
title: "تعداد LineCapType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Drawing.LineCapType enum. يمثل نهايات الخط"
type: docs
url: /ar/net/aspose.cells.drawing/linecaptype/
---
## LineCapType enumeration

يمثل نهايات الخط.

```csharp
public enum LineCapType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Square | `0` | المربع يبرز نصف عرض الخط. |
| Round | `1` | نهايات مستديرة. |
| Flat | `2` | الخط ينتهي عند نقطة النهاية. |
| None | `3` | بدون غطاء |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassLineCapTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 50, 100);
            
            LineFormat lineFmt = shape.Line;
            lineFmt.CapType = LineCapType.Flat;
            lineFmt.Weight = 2.0;
            lineFmt.DashStyle = MsoLineDashStyle.Solid;
            
            workbook.Save("LineCapTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


