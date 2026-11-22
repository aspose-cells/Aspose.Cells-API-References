---
title: "التعداد TextStrikeType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.TextStrikeType. يحدد هذا النوع نوع الخط المشطوب"
type: docs
url: /ar/net/aspose.cells/textstriketype/
---
## TextStrikeType enumeration

هذا النوع يحدد نوع الضربة.

```csharp
public enum TextStrikeType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Single | `0` | خط مشطوب واحد يُطبق على النص. |
| Double | `1` | خط مشطوب مزدوج يُطبق على النص. يعمل فقط على نص الأشكال أو المخططات. |
| None | `2` | لم يُطبق أي خط مشطوب على النص. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TextStrikeTypeDemo
    {
        public static void TextStrikeTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            // احصل على مرجع ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            // الوصول إلى الخلية "A1" من ورقة العمل
            Cell cell = worksheet.Cells["A1"];
            // إضافة قيمة إلى الخلية "A1"
            cell.PutValue("Hello Aspose!");

            // الوصول إلى خط الخلية
            Style style = cell.GetStyle();
            Font font = style.Font;

            // تعيين نوع الخط المشطوب إلى واحد
            font.StrikeType = TextStrikeType.Single;

            // تطبيق النمط على الخلية
            cell.SetStyle(style);

            // احفظ المصنف
            workbook.Save("TextStrikeTypeExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


