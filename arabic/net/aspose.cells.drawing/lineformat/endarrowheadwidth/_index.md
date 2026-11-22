---
title: "LineFormat.EndArrowheadWidth"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LineFormat. تحصل وتعيّن نوع عرض السهم النهائي للخط"
type: docs
url: /ar/net/aspose.cells.drawing/lineformat/endarrowheadwidth/
---
## LineFormat.EndArrowheadWidth property

يحصل على ويضبط نوع عرض السهم النهائي للخط.

```csharp
public MsoArrowheadWidth EndArrowheadWidth { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyEndArrowheadWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكل خط
            Shape line = worksheet.Shapes.AddLine(10, 10, 100, 10, 5, 5);

            // احصل على تنسيق الخط
            LineFormat lineFmt = line.Line;

            // تعيين عرض السهم النهائي
            lineFmt.EndArrowheadWidth = MsoArrowheadWidth.Medium;

            // احفظ المصنف
            workbook.Save("LineFormatPropertyEndArrowheadWidthDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


