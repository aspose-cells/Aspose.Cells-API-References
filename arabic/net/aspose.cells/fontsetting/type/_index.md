---
title: "FontSetting.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FontSetting. تحصل على نوع عقدة النص"
type: docs
url: /ar/net/aspose.cells/fontsetting/type/
---
## FontSetting.Type property

يحصل على نوع عقدة النص.

```csharp
public virtual TextNodeType Type { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;  // Added this using directive
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingPropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة نص إلى خلية
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // الحصول على إعدادات الخط لأحرف الخلية
            FontSetting fontSetting = new FontSetting(0, 6, workbook.Worksheets);

            // عرض قيمة Type الحالية
            Console.WriteLine("Current Type value: " + fontSetting.Type);

            // إظهار كيف يؤثر Type على معالجة النص
            if (fontSetting.Type == TextNodeType.TextRun)
            {
                Console.WriteLine("The text is a standard text run.");
            }
            else if (fontSetting.Type == TextNodeType.TextParagraph)
            {
                Console.WriteLine("The text is part of a paragraph.");
            }
            else if (fontSetting.Type == TextNodeType.Equation)
            {
                Console.WriteLine("The text represents an equation.");
            }

            // تطبيق تنسيق مختلف بناءً على Type
            if (fontSetting.Type == TextNodeType.TextRun)
            {
                fontSetting.Font.Color = System.Drawing.Color.Red;
                fontSetting.SetWordArtStyle(PresetWordArtStyle.WordArtStyle1);
            }

            // حفظ النتيجة
            workbook.Save("FontSettingTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [TextNodeType](../../../aspose.cells.drawing.texts/textnodetype/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


