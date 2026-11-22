---
title: "LineFormat.BeginArrowheadLength"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LineFormat. يحصل ويضبط نوع طول السهم الابتدائي للخط"
type: docs
url: /ar/net/aspose.cells.drawing/lineformat/beginarrowheadlength/
---
## LineFormat.BeginArrowheadLength property

يحصل على ويضبط نوع طول السهم الابتدائي للخط.

```csharp
public MsoArrowheadLength BeginArrowheadLength { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyBeginArrowheadLengthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكل خط
            Shape lineShape = worksheet.Shapes.AddLine(1, 1, 100, 100, 5, 5);
            LineShape line = (LineShape)lineShape;

            // تعيين طول رأس السهم الابتدائي
            line.Line.BeginArrowheadLength = MsoArrowheadLength.Long;

            // احفظ المصنف
            workbook.Save("LineFormatPropertyBeginArrowheadLengthDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


