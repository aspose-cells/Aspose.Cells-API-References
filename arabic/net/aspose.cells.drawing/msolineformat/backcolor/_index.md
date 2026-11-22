---
title: "MsoLineFormat.BackColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MsoLineFormat. تحصل وتعيّن لون خلفية خط الحدود"
type: docs
url: /ar/net/aspose.cells.drawing/msolineformat/backcolor/
---
## MsoLineFormat.BackColor property

يحصل على ويضبط لون خلفية خط الحدود.

```csharp
public Color BackColor { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyBackColorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكل خط
            Shape line = worksheet.Shapes.AddLine(1, 1, 100, 100, 5, 5);

            // حدد خصائص الخط
            line.LineFormat.ForeColor = Color.Red;
            line.LineFormat.BackColor = Color.Yellow; // Demonstrating BackColor usage
            line.LineFormat.DashStyle = MsoLineDashStyle.Solid;
            line.LineFormat.Weight = 2.0;

            // احفظ المصنف
            workbook.Save("LineFormatBackColorDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


