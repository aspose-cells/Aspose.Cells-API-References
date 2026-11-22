---
title: "Shape.MacroName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تحصل وتعيّن اسم الماكرو"
type: docs
url: /ar/net/aspose.cells.drawing/shape/macroname/
---
## Shape.MacroName property

يحصل ويضبط اسم الماكرو.

```csharp
public string MacroName { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyMacroNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل إلى ورقة العمل
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // تعيين اسم الماكرو للشكل
            shape.MacroName = "DoWork()";

            // إخراج التأكيد
            Console.WriteLine("Shape macro name set to: " + shape.MacroName);
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


