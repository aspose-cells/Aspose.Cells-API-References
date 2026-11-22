---
title: "TextEffectFormat.SetTextEffect"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة TextEffectFormat. تعيين تأثير النص المسبق"
type: docs
url: /ar/net/aspose.cells.drawing/texteffectformat/settexteffect/
---
## TextEffectFormat.SetTextEffect method

يضبط تأثير النص المحدد مسبقًا.

```csharp
public void SetTextEffect(MsoPresetTextEffect effect)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تأثير | MsoPresetTextEffect | تأثير النص المحدد مسبقًا. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TextEffectFormatMethodSetTextEffectWithMsoPresetTextEffectDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً لـ WordArt
            Shape wordArt = worksheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", "Arial", 36, false, false, 0, 0, 0, 0, 100, 100);

            // احصل على TextEffectFormat للشكل
            TextEffectFormat textEffectFormat = wordArt.TextEffect;

            try
            {
                // استدعِ طريقة SetTextEffect مع معامل MsoPresetTextEffect
                textEffectFormat.SetTextEffect(MsoPresetTextEffect.TextEffect10);

                // عيّن خصائص إضافية لـ WordArt
                textEffectFormat.FontBold = true;
                textEffectFormat.FontItalic = false;
                textEffectFormat.FontSize = 24;

                Console.WriteLine("SetTextEffect method executed successfully with MsoPresetTextEffect.TextEffect10");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTextEffect method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("TextEffectFormatMethodSetTextEffectWithMsoPresetTextEffectDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [MsoPresetTextEffect](../../msopresettexteffect/)
* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


