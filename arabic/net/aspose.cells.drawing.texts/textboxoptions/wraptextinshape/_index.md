---
title: "TextBoxOptions.WrapTextInShape"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextBoxOptions. تحدد التفاف النص داخل الشكل. False لا يحدث أي التفاف على نص الجسم. True يحدث التفاف على نص الجسم"
type: docs
url: /ar/net/aspose.cells.drawing.texts/textboxoptions/wraptextinshape/
---
## TextBoxOptions.WrapTextInShape property

يحدد تغليف النص داخل الشكل. False - لن يحدث تغليف على جسم النص. True - سيحدث تغليف على جسم النص.

```csharp
public bool WrapTextInShape { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyWrapTextInShapeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل صندوق نص مع المعلمات الصحيحة
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);

            // حدد النص الذي سيتفاف داخل الشكل
            textBox.Text = "This is a long text that should wrap within the text box shape boundaries when WrapTextInShape is enabled.";

            // تمكين التفاف النص داخل الشكل
            textBox.TextBoxOptions.WrapTextInShape = true;

            // احفظ المصنف
            workbook.Save("TextBoxWrapTextDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


