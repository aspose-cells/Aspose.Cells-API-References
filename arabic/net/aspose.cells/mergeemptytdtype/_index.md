---
title: "التعداد MergeEmptyTdType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.MergeEmptyTdType. يمثل نوع الدمج لعنصر TD فارغ عند تصدير ملف إلى HTML"
type: docs
url: /ar/net/aspose.cells/mergeemptytdtype/
---
## MergeEmptyTdType enumeration

يمثل نوع الدمج لعنصر TD فارغ عند تصدير ملف إلى HTML.

```csharp
public enum MergeEmptyTdType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Default | `0` | عرض مشابه لـ MS Excel. |
| None | `1` | لن يتم دمج عناصر TD الفارغة عند تصدير الملف إلى html. سيؤدي ذلك إلى إنشاء ملف html أكبر بشكل كبير. |
| MergeForcely | `2` | دمج عنصر TD الفارغ بشكل إجباري عند تصدير الملف إلى html. سيقل حجم ملف html بشكل كبير بعد ضبط القيمة إلى true. إذا كنت ترغب في استيراد ملف html إلى Excel أو تصدير خطوط شبكة مثالية عند حفظ الملف إلى html، يرجى الحفاظ على القيمة الافتراضية. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MergeEmptyTdTypeDemo
    {
        public static void MergeEmptyTdTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Data1");
            worksheet.Cells["B1"].PutValue("Data2");
            worksheet.Cells["C1"].PutValue("Data3");

            // إنشاء HtmlSaveOptions وتعيين خاصية MergeEmptyTdType
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.MergeEmptyTdType = MergeEmptyTdType.MergeForcely;

            // حفظ المصنف بتنسيق HTML
            workbook.Save("MergeEmptyTdTypeExample.html", saveOptions);

            Console.WriteLine("HTML file saved with MergeEmptyTdType.MergeForcely option.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


