---
title: "Enum FontSchemeType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.FontSchemeType enum. يمثل نوع المخطط للخط"
type: docs
url: /ar/net/aspose.cells/fontschemetype/
---
## FontSchemeType enumeration

يمثل نوع مخطط الخط.

```csharp
public enum FontSchemeType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | لا شيء |
| Major | `1` | مخطط رئيسي. |
| Minor | `2` | مخطط فرعي. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontSchemeTypeDemo
    {
        public static void FontSchemeTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            // احصل على مرجع ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            // الوصول إلى الخلية "A1" من ورقة العمل
            Cell cell = worksheet.Cells["A1"];
            // إضافة قيمة إلى الخلية "A1"
            cell.PutValue("Hello Aspose!");

            // الوصول إلى خط نمط الخلية
            Aspose.Cells.Font font = cell.GetStyle().Font;

            // تعيين نوع مخطط الخط إلى رئيسي
            font.SchemeType = FontSchemeType.Major;

            // تعيين خصائص خط أخرى للعرض
            font.Name = "Arial";
            font.Size = 14;
            font.Color = System.Drawing.Color.Blue;

            // احفظ المصنف
            workbook.Save("FontSchemeTypeExample.xlsx");
            workbook.Save("FontSchemeTypeExample.pdf");
            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


