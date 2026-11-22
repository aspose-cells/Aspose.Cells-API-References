---
title: "Shape.AnchorType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. يحصل ويضبط نوع عنصر نائب لمرساة الشكل"
type: docs
url: /ar/net/aspose.cells.drawing/shape/anchortype/
---
## Shape.AnchorType property

يحصل ويضبط نوع عنصر نائب مرساة shape.

```csharp
public ShapeAnchorType AnchorType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyAnchorTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً بنوع مرساة افتراضي
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 0, 0);
            
            // تحقق وعدل نوع المرساة
            if (shape.AnchorType == ShapeAnchorType.OneCellAnchor)
            {
                shape.AnchorType = ShapeAnchorType.TwoCellAnchor;
                Console.WriteLine("Anchor type changed to TwoCellAnchor");
            }
            
            // احفظ المصنف
            workbook.Save("ShapeAnchorTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ShapeAnchorType](../../shapeanchortype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


