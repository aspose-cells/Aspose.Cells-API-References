---
title: "ShapeTextAlignment.IsLockedText"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ShapeTextAlignment. تشير إلى ما إذا كان الشكل مقفلًا عندما تكون ورقة العمل محمية"
type: docs
url: /ar/net/aspose.cells.drawing.texts/shapetextalignment/islockedtext/
---
## ShapeTextAlignment.IsLockedText property

يشير إلى ما إذا كان الشكل مقفلًا عندما تكون ورقة العمل محمية.

```csharp
public bool IsLockedText { get; set; }
```

### ملاحظات

يعمل فقط عندما تكون ورقة العمل محمية.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyIsLockedTextDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة مربع نص إلى ورقة العمل
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
            textBox.Text = "Sample Text";

            // الوصول إلى خصائص محاذاة النص
            Aspose.Cells.Drawing.Texts.ShapeTextAlignment textAlignment = textBox.TextBody.TextAlignment;

            // تعيين وإظهار خاصية IsLockedText
            textAlignment.IsLockedText = true;
            Console.WriteLine("Text locked status: " + textAlignment.IsLockedText);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


