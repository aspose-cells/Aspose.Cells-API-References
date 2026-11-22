---
title: "Shape.TextDirection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. يحصل/يضبط اتجاه تدفق النص لهذا الكائن"
type: docs
url: /ar/net/aspose.cells.drawing/shape/textdirection/
---
## Shape.TextDirection property

يحصل/يضبط اتجاه تدفق النص لهذا الكائن.

```csharp
public TextDirectionType TextDirection { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextDirectionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل مربع نص
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 0, 100, 100, 100);
            shape.Text = "Sample Text";

            // تعيين وعرض خاصية TextDirection
            shape.TextDirection = TextDirectionType.Context;
            Console.WriteLine("Initial TextDirection: " + shape.TextDirection);

            // تغيير اتجاه النص
            shape.TextDirection = TextDirectionType.LeftToRight;
            Console.WriteLine("Updated TextDirection: " + shape.TextDirection);

            // احفظ المصنف
            workbook.Save("TextDirectionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [TextDirectionType](../../../aspose.cells/textdirectiontype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


