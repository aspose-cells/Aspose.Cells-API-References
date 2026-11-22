---
title: "AutoFitterOptions.DefaultEditLanguage"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AutoFitterOptions. تحصل أو تعيين لغة التحرير الافتراضية"
type: docs
url: /ar/net/aspose.cells/autofitteroptions/defaulteditlanguage/
---
## AutoFitterOptions.DefaultEditLanguage property

يحصل أو يضبط لغة التحرير الافتراضية.

```csharp
public DefaultEditLanguage DefaultEditLanguage { get; set; }
```

### ملاحظات

قد يعرض/يرسم تخطيطات مختلفة لفقرة النص عندما يتم تعيين لغات تحرير مختلفة. الافتراضي هو Auto.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyDefaultEditLanguageDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين نص CJK تجريبي في خلية
            worksheet.Cells["A1"].PutValue("日本語のテキスト");

            AutoFitterOptions options = new AutoFitterOptions();
            options.DefaultEditLanguage = DefaultEditLanguage.CJK;

            // ضبط تلقائي للصف مع إعدادات لغة CJK
            worksheet.AutoFitRows(options);

            Console.WriteLine("Auto-fit completed with DefaultEditLanguage: " + options.DefaultEditLanguage);
            workbook.Save("DefaultEditLanguageDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [DefaultEditLanguage](../../defaulteditlanguage/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


