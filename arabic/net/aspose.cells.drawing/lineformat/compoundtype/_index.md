---
title: "LineFormat.CompoundType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LineFormat. تحدد نوع تجميع الخط"
type: docs
url: /ar/net/aspose.cells.drawing/lineformat/compoundtype/
---
## LineFormat.CompoundType property

يحدد نوع مركب الخط.

```csharp
public MsoLineStyle CompoundType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyCompoundTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكل خط
            Shape line = worksheet.Shapes.AddLine(1, 1, 100, 100, 5, 5);

            // احصل على تنسيق الخط
            LineFormat lineFmt = line.Line;

            // تعيين نوع المركب
            lineFmt.CompoundType = MsoLineStyle.Single;

            // احفظ المصنف
            workbook.Save("LineFormatCompoundTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [MsoLineStyle](../../msolinestyle/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


