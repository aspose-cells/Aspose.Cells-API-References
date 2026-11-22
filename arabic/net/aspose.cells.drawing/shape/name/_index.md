---
title: "Shape.Name"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية الشكل. تحصل وتعيّن اسم الشكل"
type: docs
url: /ar/net/aspose.cells.drawing/shape/name/
---
## Shape.Name property

يحصل على ويضبط اسم الشكل.

```csharp
public string Name { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف شكلاً وقم بتعيين اسمه
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
            shape.Name = "shape1";
            
            // تحقق من أن الاسم تم ضبطه
            Console.WriteLine("Shape name: " + shape.Name);
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


