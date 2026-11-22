---
title: "LineFormat.JoinType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LineFormat. يحدد نوع وصل الخط"
type: docs
url: /ar/net/aspose.cells.drawing/lineformat/jointype/
---
## LineFormat.JoinType property

يحدد نوع وصل الخط.

```csharp
public LineJoinType JoinType { get; set; }
```

### أمثلة

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyJoinTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء شكل خط
            LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // تعيين نوع وصل الخط إلى دائري
            line.Line.JoinType = LineJoinType.Round;

            // احفظ المصنف
            workbook.Save("LineJoinTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [LineJoinType](../../linejointype/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


