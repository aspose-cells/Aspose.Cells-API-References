---
title: "TextEffectFormat.FontBold"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextEffectFormat. تشير إلى ما إذا كان الخط غامقًا"
type: docs
url: /ar/net/aspose.cells.drawing/texteffectformat/fontbold/
---
## TextEffectFormat.FontBold property

يشير إلى ما إذا كان الخط عريضًا.

```csharp
public bool FontBold { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyFontBoldDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل مربع نص (يرجع كائن TextBox مباشرة)
            TextBox textbox = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 200, 100);
            textbox.Text = "Sample Text";

            // احصل على تنسيق تأثير النص
            TextEffectFormat effFormat = textbox.TextEffect;

            // تعيين خصائص الخط بما في ذلك الغامق
            effFormat.FontName = "Arial";
            effFormat.FontBold = true;
            effFormat.FontItalic = false;
            effFormat.FontSize = 14;

            // احفظ المصنف
            workbook.Save("TextEffectFormatFontBoldDemo.xlsx");

            Console.WriteLine("Text effect format with bold font applied successfully.");
        }
    }
}
```

### انظر أيضًا

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


