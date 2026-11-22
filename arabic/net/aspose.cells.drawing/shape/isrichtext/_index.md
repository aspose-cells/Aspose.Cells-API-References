---
title: "Shape.IsRichText"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. ما إذا كان النص نصًا غنيًا أم لا"
type: docs
url: /ar/net/aspose.cells.drawing/shape/isrichtext/
---
## Shape.IsRichText property

ما إذا كان النص نصًا غنيًا أم لا.

```csharp
public bool IsRichText { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsRichTextDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً بنص
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
            shape.Text = "This is <b>rich</b> text";

            // تحقق مما إذا كان النص نصًا غنيًا
            if (shape.IsRichText)
            {
                Console.WriteLine("The text is rich text.");
            }
            else
            {
                Console.WriteLine("The text is not rich text.");
            }
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


