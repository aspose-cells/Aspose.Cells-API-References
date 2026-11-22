---
title: "Shape.IsTextWrapped"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. يحصل على ويضبط نوع التفاف النص للشكل الذي يحتوي على نص"
type: docs
url: /ar/net/aspose.cells.drawing/shape/istextwrapped/
---
## Shape.IsTextWrapped property

يحصل أو يحدد نوع التفاف النص للشكل الذي يحتوي على نص.

```csharp
public bool IsTextWrapped { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsTextWrappedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً واضبط بعض النص
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
            shape.Text = "This is a sample text that will demonstrate text wrapping functionality";

            // عرض خاصية IsTextWrapped
            Console.WriteLine("Initial IsTextWrapped value: " + shape.IsTextWrapped);
            
            // بدّل تغليف النص
            shape.IsTextWrapped = !shape.IsTextWrapped;
            Console.WriteLine("After toggle, IsTextWrapped value: " + shape.IsTextWrapped);

            // احفظ المصنف
            workbook.Save("ShapeTextWrappingDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


