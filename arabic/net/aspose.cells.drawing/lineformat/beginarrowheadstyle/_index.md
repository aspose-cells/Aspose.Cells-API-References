---
title: "LineFormat.BeginArrowheadStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LineFormat. يحصل ويضبط نوع السهم الابتدائي للخط"
type: docs
url: /ar/net/aspose.cells.drawing/lineformat/beginarrowheadstyle/
---
## LineFormat.BeginArrowheadStyle property

يحصل على ويضبط نوع السهم الابتدائي للخط.

```csharp
public MsoArrowheadStyle BeginArrowheadStyle { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyBeginArrowheadStyleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكل خط
            Shape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // تعيين نمط رأس السهم الابتدائي
            line.Line.BeginArrowheadStyle = MsoArrowheadStyle.ArrowOpen;

            // احفظ المصنف
            workbook.Save("LineFormatPropertyBeginArrowheadStyleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [MsoArrowheadStyle](../../msoarrowheadstyle/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


