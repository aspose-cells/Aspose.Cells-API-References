---
title: "TextBoxOptions.AllowTextToOverflow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextBoxOptions. ما إذا كان يسمح للنص بالتجاوز خارج الشكل"
type: docs
url: /ar/net/aspose.cells.drawing.texts/textboxoptions/allowtexttooverflow/
---
## TextBoxOptions.AllowTextToOverflow property

ما إذا كان يُسمح للنص بتجاوز الشكل.

```csharp
public bool AllowTextToOverflow { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyAllowTextToOverflowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة مربع نص إلى ورقة العمل
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);

            // حدد النص الذي قد يتجاوز
            textBox.Text = "This is a long text that might overflow the text box boundaries if AllowTextToOverflow is false";

            // تمكين تجاوز النص
            textBox.TextBoxOptions.AllowTextToOverflow = true;

            // احفظ المصنف
            workbook.Save("TextBoxAllowTextToOverflowDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


