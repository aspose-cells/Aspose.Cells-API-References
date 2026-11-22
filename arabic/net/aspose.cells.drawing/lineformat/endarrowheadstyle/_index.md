---
title: "LineFormat.EndArrowheadStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LineFormat. تحصل وتضبط نوع السهم النهائي للخط"
type: docs
url: /ar/net/aspose.cells.drawing/lineformat/endarrowheadstyle/
---
## LineFormat.EndArrowheadStyle property

يحصل على ويضبط نوع السهم النهائي للخط.

```csharp
public MsoArrowheadStyle EndArrowheadStyle { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyEndArrowheadStyleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكل خط
            Aspose.Cells.Drawing.LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // احصل على تنسيق الخط
            LineFormat lineFmt = line.Line;

            // اضبط نمط رأس السهم النهائي
            lineFmt.EndArrowheadStyle = MsoArrowheadStyle.ArrowOpen;

            // احفظ المصنف
            workbook.Save("LineFormatPropertyEndArrowheadStyleDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [MsoArrowheadStyle](../../msoarrowheadstyle/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


