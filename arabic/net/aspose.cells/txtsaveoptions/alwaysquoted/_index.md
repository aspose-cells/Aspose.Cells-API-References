---
title: "TxtSaveOptions.AlwaysQuoted"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TxtSaveOptions. تشير إلى ما إذا كان يتم دائمًا إضافة  لكل حقل. إذا كانت true فستُقتبس جميع القيم. إذا كانت false فستُقتبس القيم فقط عند الحاجة، على سبيل المثال عندما تحتوي القيم على أحرف خاصة مثل   n أو حرف الفاصل. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/txtsaveoptions/alwaysquoted/
---
## TxtSaveOptions.AlwaysQuoted property

تشير إلى ما إذا كان يتم دائمًا إضافة '\"' لكل حقل. إذا كانت true فستُقتبس جميع القيم؛ إذا كانت false فستُقتبس القيم فقط عند الحاجة (على سبيل المثال، عندما تحتوي القيم على أحرف خاصة مثل '\"' ، '\\n' أو حرف الفاصل). القيمة الافتراضية هي false.

```csharp
[Obsolete("Use QuoteType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool AlwaysQuoted { get; set; }
```

### ملاحظات

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام خاصية QuoteType. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أغسطس 2012. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyAlwaysQuotedDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200.50);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(899.99);

            // إنشاء TxtSaveOptions مع تعيين AlwaysQuoted إلى true
            TxtSaveOptions saveOptions = new TxtSaveOptions
            {
                Separator = ',',
                AlwaysQuoted = true,
                QuoteType = TxtValueQuoteType.Always
            };

            // حفظ مع وضع علامات اقتباس حول جميع القيم
            workbook.Save("AlwaysQuoted_True.txt", saveOptions);

            // تغيير إلى false وحفظ مرة أخرى
            saveOptions.AlwaysQuoted = false;
            workbook.Save("AlwaysQuoted_False.txt", saveOptions);

            Console.WriteLine("Files saved with different AlwaysQuoted settings.");
        }
    }
}
```

### انظر أيضًا

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


