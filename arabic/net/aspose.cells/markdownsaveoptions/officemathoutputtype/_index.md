---
title: "MarkdownSaveOptions.OfficeMathOutputType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MarkdownSaveOptions. تشير إلى كيفية تصدير كائنات OfficeMath إلى Markdown. القيمة الافتراضية هي Image"
type: docs
url: /ar/net/aspose.cells/markdownsaveoptions/officemathoutputtype/
---
## MarkdownSaveOptions.OfficeMathOutputType property

يحدد كيفية تصدير كائنات OfficeMath إلى Markdown، القيمة الافتراضية هي Image.

```csharp
public HtmlOfficeMathOutputType OfficeMathOutputType { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyOfficeMathOutputTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات عينة تشمل صيغة قد تحتوي على OfficeMath
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].Formula = "=SQRT(16)";

            try
            {
                // إنشاء خيارات حفظ Markdown
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // عرض القيمة الحالية لـ OfficeMathOutputType
                Console.WriteLine("Current OfficeMathOutputType: " + saveOptions.OfficeMathOutputType);

                // تعيين OfficeMathOutputType إلى MathML
                saveOptions.OfficeMathOutputType = HtmlOfficeMathOutputType.MathML;
                Console.WriteLine("Changed OfficeMathOutputType to: " + saveOptions.OfficeMathOutputType);

                // حفظ المصنف باستخدام نوع الإخراج MathML
                workbook.Save("OfficeMathOutputType_MathML.md", saveOptions);

                // تغيير إلى نوع الإخراج Image
                saveOptions.OfficeMathOutputType = HtmlOfficeMathOutputType.Image;
                Console.WriteLine("Changed OfficeMathOutputType to: " + saveOptions.OfficeMathOutputType);

                // حفظ المصنف باستخدام نوع الإخراج Image
                workbook.Save("OfficeMathOutputType_Image.md", saveOptions);

                Console.WriteLine("OfficeMathOutputType demonstration completed successfully.");
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

* enum [HtmlOfficeMathOutputType](../../htmlofficemathoutputtype/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


