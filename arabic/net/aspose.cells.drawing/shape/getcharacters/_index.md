---
title: "Shape.GetCharacters"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Shape. تُرجع جميع كائنات Characters التي تمثل نطاقًا من الأحرف داخل النص"
type: docs
url: /ar/net/aspose.cells.drawing/shape/getcharacters/
---
## Shape.GetCharacters method

يرجع جميع كائنات Characters التي تمثل نطاقًا من الأحرف داخل النص.

```csharp
[Obsolete("Use Shape.GetRichFormattings() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList GetCharacters()
```

### قيمة الإرجاع

جميع كائنات Characters

### ملاحظات

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة Shape.GetRichFormattings(). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ نوفمبر 2023. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using System.Collections;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetCharactersDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل مربع نص إلى ورقة العمل مع جميع المعلمات المطلوبة
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
            shape.Text = "Sample Text";

            // الحصول على الأحرف من الشكل
            ArrayList characters = shape.GetCharacters();

            // عرض معلومات حول كل حرف
            foreach (FontSetting charSetting in characters)
            {
                Console.WriteLine($"Font: {charSetting.Font.Name}, Size: {charSetting.Font.Size}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


