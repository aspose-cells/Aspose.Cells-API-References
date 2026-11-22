---
title: "Shape.TextVerticalOverflow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تحصل وتضبط نوع الفائض العمودي للنص في الشكل الذي يحتوي على نص"
type: docs
url: /ar/net/aspose.cells.drawing/shape/textverticaloverflow/
---
## Shape.TextVerticalOverflow property

يحصل ويضبط نوع تدفق النص العمودي للشكل الذي يحتوي على نص.

```csharp
public TextOverflowType TextVerticalOverflow { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextVerticalOverflowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل مستطيل
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);
            
            // تعيين النص وجعله يتجاوز عموديًا
            shape.Text = "This is a long text that will demonstrate vertical text overflow functionality in the shape.";
            shape.TextVerticalOverflow = TextOverflowType.Overflow;

            // احفظ المصنف
            workbook.Save("ShapeTextVerticalOverflowDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [TextOverflowType](../../textoverflowtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


