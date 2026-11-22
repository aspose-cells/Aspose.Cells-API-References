---
title: "Shape.LinkedCell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تحصل أو تضبط نطاق الورقة المرتبط بقيمة التحكم"
type: docs
url: /ar/net/aspose.cells.drawing/shape/linkedcell/
---
## Shape.LinkedCell property

يحصل على أو يضبط نطاق الورقة المرتبط بقيمة التحكم.

```csharp
public string LinkedCell { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLinkedCellDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل إلى ورقة العمل
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // قم بتعيين خاصية LinkedCell إلى B6
            shape.LinkedCell = "$B$6";

            // غيّر LinkedCell إلى A1 إذا كان B6
            if (shape.LinkedCell.Equals("$B$6"))
            {
                shape.LinkedCell = "A1";
            }

            // أخرج القيمة الحالية لـ LinkedCell
            Console.WriteLine("Shape's LinkedCell: " + shape.LinkedCell);
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


