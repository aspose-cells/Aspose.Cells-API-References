---
title: "LineFormat.BeginArrowheadWidth"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LineFormat. تحصل وتعيّن نوع عرض السهم الابتدائي للخط"
type: docs
url: /ar/net/aspose.cells.drawing/lineformat/beginarrowheadwidth/
---
## LineFormat.BeginArrowheadWidth property

يحصل على ويضبط نوع عرض السهم الابتدائي للخط.

```csharp
public MsoArrowheadWidth BeginArrowheadWidth { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyBeginArrowheadWidthDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكل خط
            Shape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 10);

            // تعيين خصائص تنسيق الخط
            LineFormat lineFmt = line.Line;
            lineFmt.BeginArrowheadWidth = MsoArrowheadWidth.Medium;
            lineFmt.EndArrowheadWidth = MsoArrowheadWidth.Medium;

            // احفظ المصنف
            workbook.Save("LineFormatDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


