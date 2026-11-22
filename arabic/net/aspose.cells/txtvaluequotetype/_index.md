---
title: "تعداد TxtValueQuoteType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.TxtValueQuoteType تعداد. يحدد نوع استخدام علامات الاقتباس للقيم في ملفات النص ذات التنسيق"
type: docs
url: /ar/net/aspose.cells/txtvaluequotetype/
---
## TxtValueQuoteType enumeration

يحدد نوع استخدام علامات الاقتباس للقيم في ملفات النص المنسقة.

```csharp
public enum TxtValueQuoteType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Normal | `0` | جميع القيم التي تحتوي على أحرف خاصة مثل علامة الاقتباس، حرف الفاصل سيتم اقتباسها. نفس سلوك مايكروسوفت إكسل لتصدير ملف نصي. |
| Always | `1` | جميع القيم سيتم اقتباسها دائمًا. |
| Minimum | `2` | اقتبس القيم فقط عند الحاجة. على سبيل المثال، إذا كانت قيمة واحدة تحتوي على علامة اقتباس ولكن علامة الاقتباس ليست في بداية هذه القيمة، فلن يتم اقتباس هذه القيمة. |
| Never | `3` | جميع القيم لن يتم اقتباسها. قد لا يتم قراءة ملف النص المُصدَّر بهذا النوع بشكل صحيح لأن علامات الاقتباس المطلوبة غائبة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TxtValueQuoteTypeDemo
    {
        public static void TxtValueQuoteTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات إلى ورقة العمل
            worksheet.Cells[0, 0].Value = "Name";
            worksheet.Cells[0, 1].Value = "Age";
            worksheet.Cells[1, 0].Value = "John Doe";
            worksheet.Cells[1, 1].Value = 30;
            worksheet.Cells[2, 0].Value = "Jane Smith";
            worksheet.Cells[2, 1].Value = 25;

            // إنشاء TxtSaveOptions وتعيين QuoteType
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.QuoteType = TxtValueQuoteType.Always;

            // احفظ المصنف كملف نصي باستخدام نوع الاقتباس المحدد
            workbook.Save("TxtValueQuoteTypeExample.txt", saveOptions);

            Console.WriteLine("Workbook saved with TxtValueQuoteType.Always");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


