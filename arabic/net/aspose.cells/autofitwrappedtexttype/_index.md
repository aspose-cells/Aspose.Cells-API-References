---
title: "تعداد AutoFitWrappedTextType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.AutoFitWrappedTextType. يمثل نوع النص الملتف المتكيف تلقائيًا"
type: docs
url: /ar/net/aspose.cells/autofitwrappedtexttype/
---
## AutoFitWrappedTextType enumeration

يمثل نوع الضبط التلقائي للنص الملتف.

```csharp
public enum AutoFitWrappedTextType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Default | `0` | يعمل مثل MS Excel. |
| Paragraph | `1` | تعديل العرض تلقائيًا مع أطول فقرة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;

    public class AutoFitWrappedTextTypeDemo
    {
        public static void AutoFitWrappedTextTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].PutValue("This is a sample text that will be wrapped and auto-fitted.\r\n This is a sample text that will be wrapped and auto-fitted. This is a sample text that will be wrapped and auto-fitted. This is a sample text that will be wrapped and auto-fitted.");
            worksheet.Cells["A5"].PutValue("Another sample text to demonstrate \r\n auto-fitting wrapped text. Another sample text to demonstrate auto-fitting wrapped text.\r\n Another sample text to demonstrate auto-fitting wrapped text. Another sample text to demonstrate auto-fitting wrapped text.");

            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);

            Style style2 = worksheet.Cells["A5"].GetStyle();
            style2.IsTextWrapped = true;
            worksheet.Cells["A5"].SetStyle(style);

            // إنشاء نطاق A1:F3
            Range range = worksheet.Cells.CreateRange(0, 0, 3, 6);
            // دمج الخلايا
            range.Merge();

            // إنشاء نطاق A4:F6
            Range range2 = worksheet.Cells.CreateRange(4, 0, 3, 6);
            // دمج الخلايا
            range2.Merge();

            // إنشاء AutoFitterOptions وتعيين AutoFitWrappedTextType
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph;

            // تعديل الصفوف تلقائيًا باستخدام الخيارات المحددة
            worksheet.AutoFitRows(options);

            // احفظ المصنف
            workbook.Save("AutoFitWrappedTextTypeExample.xlsx");
            workbook.Save("AutoFitWrappedTextTypeExample.pdf");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


