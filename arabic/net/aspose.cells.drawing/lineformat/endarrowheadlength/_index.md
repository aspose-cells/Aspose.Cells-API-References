---
title: "LineFormat.EndArrowheadLength"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LineFormat. يحصل ويضبط نوع طول السهم النهائي للخط"
type: docs
url: /ar/net/aspose.cells.drawing/lineformat/endarrowheadlength/
---
## LineFormat.EndArrowheadLength property

يحصل على ويضبط نوع طول السهم النهائي للخط.

```csharp
public MsoArrowheadLength EndArrowheadLength { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyEndArrowheadLengthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل خط والحصول على كائن الشكل مباشرة
            LineShape line = (LineShape)worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 10);

            // تعيين طول رأس السهم النهائي
            line.Line.EndArrowheadLength = MsoArrowheadLength.Long;

            // احفظ المصنف
            workbook.Save("LineFormatPropertyEndArrowheadLengthDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


