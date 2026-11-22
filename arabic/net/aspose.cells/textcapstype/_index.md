---
title: "تعداد TextCapsType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.TextCapsType. يحدد هذا النوع أنواع الحروف الكبيرة للنص"
type: docs
url: /ar/net/aspose.cells/textcapstype/
---
## TextCapsType enumeration

هذا النوع يحدد أنواع القمة للنص.

```csharp
public enum TextCapsType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | بدون حروف كبيرة |
| All | `1` | تطبيق جميع الحروف الكبيرة على النص. |
| Small | `2` | تطبيق الحروف الصغيرة على النص. |

### ملاحظات

يمكن تطبيقه فقط على المخطط والشكل.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TextCapsTypeDemo
    {
        public static void TextCapsTypeExample()
        {
            // كود إضافي لتوضيح كيفية استخدام المثيل
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ضبط قيمة الخلية
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Hello Aspose!");

            // احصل على نمط الخلية
            Style style = cell.GetStyle();

            // ضبط نوع حروف الخط إلى جميع الحروف الكبيرة
            style.Font.CapsType = Aspose.Cells.TextCapsType.All;

            // تطبيق النمط على الخلية
            cell.SetStyle(style);

            // احفظ المصنف
            workbook.Save("TextCapsTypeExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


