---
title: "MarkdownLoadOptions.HasFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MarkdownLoadOptions. تشير إلى ما إذا كان النص صيغة إذا بدأ بـ"
type: docs
url: /ar/net/aspose.cells/markdownloadoptions/hasformula/
---
## MarkdownLoadOptions.HasFormula property

يشير إلى ما إذا كان النص صيغة إذا بدأ بـ "=".

```csharp
public bool HasFormula { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownLoadOptionsPropertyHasFormulaDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء نسخة من MarkdownLoadOptions
                MarkdownLoadOptions options = new MarkdownLoadOptions();

                // عرض القيمة الافتراضية لـ HasFormula
                Console.WriteLine($"Default HasFormula value: {options.HasFormula}");

                // تعيين HasFormula إلى true
                options.HasFormula = true;
                Console.WriteLine($"HasFormula set to: {options.HasFormula}");

                // تعيين HasFormula إلى false
                options.HasFormula = false;
                Console.WriteLine($"HasFormula set to: {options.HasFormula}");

                // إنشاء مصنف بمحتوى markdown تجريبي
                Workbook workbook = new Workbook();

                // احفظ المصنف لتوضيح إمكانية استخدام الخيارات
                workbook.Save("HasFormulaDemo.xlsx");

                Console.WriteLine("HasFormula property demonstration completed successfully.");
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

* class [MarkdownLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


