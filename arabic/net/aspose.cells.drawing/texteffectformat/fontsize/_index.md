---
title: "TextEffectFormat.FontSize"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextEffectFormat. الحجم بالنقاط للخط المستخدم في WordArt"
type: docs
url: /ar/net/aspose.cells.drawing/texteffectformat/fontsize/
---
## TextEffectFormat.FontSize property

حجم الخط (بالنقاط) المستخدم في WordArt.

```csharp
public int FontSize { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyFontSizeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة مربع نص إلى ورقة العمل
            int textboxIndex = worksheet.TextBoxes.Add(5, 5, 200, 100);
            Aspose.Cells.Drawing.TextBox textBox = worksheet.TextBoxes[textboxIndex];
            
            // تعيين النص والتنسيق
            textBox.Text = "Sample Text Effect";
            
            // احصل على تنسيق تأثير النص
            Shape shape = textBox;
            TextEffectFormat effectFormat = shape.TextEffect;
            
            // تعيين خصائص الخط بما في ذلك FontSize
            effectFormat.FontName = "Arial";
            effectFormat.FontBold = true;
            effectFormat.FontItalic = false;
            effectFormat.FontSize = 18; // Demonstrating FontSize property
            
            // احفظ المصنف
            workbook.Save("TextEffectFontSizeDemo.xlsx");
            
            Console.WriteLine("Text effect with font size 18 created successfully.");
        }
    }
}
```

### انظر أيضًا

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


