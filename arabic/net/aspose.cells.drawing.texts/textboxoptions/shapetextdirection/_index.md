---
title: "TextBoxOptions.ShapeTextDirection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextBoxOptions. يحصل أو يضبط اتجاه عرض النص داخل جسم نص معين. وهو يتطابق مع Format Shape  Text Options  Text Box  Text direction في Excel"
type: docs
url: /ar/net/aspose.cells.drawing.texts/textboxoptions/shapetextdirection/
---
## TextBoxOptions.ShapeTextDirection property

يحصل أو يضبط اتجاه عرض النص داخل جسم نص معين. يتطابق مع "Format Shape - Text Options - Text Box - Text direction" في Excel

```csharp
public TextVerticalType ShapeTextDirection { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyShapeTextDirectionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل مربع نص
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);

            // ضبط اتجاه النص إلى عمودي
            shape.TextBoxOptions.ShapeTextDirection = TextVerticalType.Vertical;

            // ضبط بعض النص لتوضيح الاتجاه
            shape.Text = "Vertical Text Example";

            // احفظ المصنف
            workbook.Save("TextBoxTextDirectionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [TextVerticalType](../../textverticaltype/)
* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


