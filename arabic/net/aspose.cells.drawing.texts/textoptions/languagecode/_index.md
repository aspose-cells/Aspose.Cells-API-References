---
title: "TextOptions.LanguageCode"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextOptions. تحصل وتضبط لغة واجهة المستخدم"
type: docs
url: /ar/net/aspose.cells.drawing.texts/textoptions/languagecode/
---
## TextOptions.LanguageCode property

يحصل على لغة واجهة المستخدم ويضبطها.

```csharp
public CountryCode LanguageCode { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextOptionsPropertyLanguageCodeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً واضبط نصه
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
            shape.Text = "Sample text with language settings";

            // اضبط رمز اللغة لخيارات نص الشكل
            shape.TextOptions.LanguageCode = CountryCode.Japan;

            // تحقق وأخرج رمز اللغة
            Console.WriteLine("Shape Text Language Code: " + shape.TextOptions.LanguageCode);

            // احفظ المصنف
            workbook.Save("TextOptionsLanguageDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [CountryCode](../../../aspose.cells/countrycode/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


