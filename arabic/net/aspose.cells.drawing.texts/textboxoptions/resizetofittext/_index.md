---
title: "TextBoxOptions.ResizeToFitText"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextBoxOptions. تشير إلى ما إذا كان يجب تغيير حجم الشكل ليتناسب مع النص"
type: docs
url: /ar/net/aspose.cells.drawing.texts/textboxoptions/resizetofittext/
---
## TextBoxOptions.ResizeToFitText property

يشير إلى ما إذا كان يجب تغيير حجم الشكل ليتناسب مع النص

```csharp
public bool ResizeToFitText { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyResizeToFitTextDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء صندوق نص مع المعلمات الصحيحة
            Aspose.Cells.Drawing.TextBox textBox = worksheet.Shapes.AddTextBox(1, 1, 100, 100, 200, 50);
            textBox.Text = "This is a sample text that will make the text box resize to fit";

            // الوصول إلى TextBoxOptions بشكل صحيح
            textBox.TextBoxOptions.ResizeToFitText = true;

            // احفظ المصنف
            workbook.Save("TextBoxResizeToFitTextDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


