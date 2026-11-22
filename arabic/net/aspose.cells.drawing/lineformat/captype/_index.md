---
title: "LineFormat.CapType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LineFormat. يحدد نهايات القمم"
type: docs
url: /ar/net/aspose.cells.drawing/lineformat/captype/
---
## LineFormat.CapType property

يحدد نهايات القبّعات.

```csharp
public LineCapType CapType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyCapTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكل خط
            LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // تعيين خصائص تنسيق الخط
            LineFormat lineFmt = line.Line;
            lineFmt.CapType = LineCapType.Flat;

            // احفظ المصنف
            workbook.Save("LineFormatCapTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [LineCapType](../../linecaptype/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


