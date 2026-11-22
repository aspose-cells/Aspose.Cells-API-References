---
title: "MarkdownSaveOptions.AlignColumnPadding"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MarkdownSaveOptions. تشير إلى ما إذا كان محاذاة الأعمدة مفعلة للجداول Markdown المُنشأة. عندما تكون مفعلة، يتم محاذاة الأعمدة عن طريق تعبئة محتوى الخلية بالحرف المحدد عادةً للمسافات. اضبطها على 0 لتعطيل محاذاة الأعمدة الافتراضية"
type: docs
url: /ar/net/aspose.cells/markdownsaveoptions/aligncolumnpadding/
---
## MarkdownSaveOptions.AlignColumnPadding property

يشير إلى ما إذا كان محاذاة الأعمدة مفعلة للجداول Markdown المُولدة. عندما تكون مفعلة، يتم محاذاة الأعمدة عن طريق تعبئة محتوى الخلية بالحرف المحدد (عادةً ' ' للمسافات). اضبطه على '\\0' لتعطيل محاذاة الأعمدة (الإعداد الافتراضي).

```csharp
public char AlignColumnPadding { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyAlignColumnPaddingDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات نموذجية لتوضيح محاذاة الأعمدة
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["C1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = "1.99";
            worksheet.Cells["C2"].Value = "10";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B3"].Value = "0.99";
            worksheet.Cells["C3"].Value = "20";

            // إنشاء مثيل MarkdownSaveOptions
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

            try
            {
                // اعرض القيمة الافتراضية لـ AlignColumnPadding
                Console.WriteLine("Default AlignColumnPadding value: '" +
                    saveOptions.AlignColumnPadding + "'");

                // اضبط AlignColumnPadding إلى حرف المسافة لمحاذاة الأعمدة
                saveOptions.AlignColumnPadding = ' ';

                // عرض القيمة المحدثة
                Console.WriteLine("Updated AlignColumnPadding value: '" +
                    saveOptions.AlignColumnPadding + "'");

                // احفظ المصنف كملف markdown مع محاذاة الأعمدة
                workbook.Save("AlignColumnPaddingDemo.md", saveOptions);
                Console.WriteLine("Markdown file saved with column alignment enabled.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


