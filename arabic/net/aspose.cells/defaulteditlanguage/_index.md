---
title: "التعداد DefaultEditLanguage"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.DefaultEditLanguage. يمثل لغة التحرير الافتراضية"
type: docs
url: /ar/net/aspose.cells/defaulteditlanguage/
---
## DefaultEditLanguage enumeration

يمثل لغة التحرير الافتراضية.

```csharp
public enum DefaultEditLanguage
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Auto | `0` | يمثل الكشف التلقائي عن لغة التحرير وفقًا للنص نفسه. |
| English | `1` | يمثل اللغة الإنجليزية. |
| CJK | `2` | يمثل اللغات الصينية واليابانية والكورية. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DefaultEditLanguageDemo
    {
        public static void DefaultEditLanguageExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء AutoFitterOptions وتعيين DefaultEditLanguage
            AutoFitterOptions autoFitterOptions = new AutoFitterOptions();
            autoFitterOptions.DefaultEditLanguage = DefaultEditLanguage.CJK;

            // تطبيق ضبط الصفوف تلقائيًا باستخدام الخيارات المحددة
            worksheet.AutoFitRows(autoFitterOptions);

            // احفظ المصنف
            workbook.Save("DefaultEditLanguageExample.xlsx");
            workbook.Save("DefaultEditLanguageExample.pdf");

            // إخراج DefaultEditLanguage المحدد إلى وحدة التحكم
            Console.WriteLine("Default Edit Language set to: " + autoFitterOptions.DefaultEditLanguage);
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


