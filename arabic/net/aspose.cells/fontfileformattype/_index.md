---
title: "تعداد FontFileFormatType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.FontFileFormatType. يمثل نوع تنسيق الخط"
type: docs
url: /ar/net/aspose.cells/fontfileformattype/
---
## FontFileFormatType enumeration

يمثل نوع تنسيق الخط.

```csharp
public enum FontFileFormatType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Unknown | `0` | نوع تنسيق الخط غير معروف. |
| Ttf | `1` | نوع تنسيق الخط TTF. |
| Otf | `2` | نوع تنسيق الخط OTF. |
| Ttc | `3` | نوع تنسيق الخط TTC. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassFontFileFormatTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى خلية وتعيين نمطها
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Font Format Type Demo");
            Style style = cell.GetStyle();

            // عرض استخدام FontFileFormatType
            FontFileFormatType fontFormat = FontFileFormatType.Ttf;
            Console.WriteLine("Selected font format: " + fontFormat.ToString());

            // تطبيق إعدادات الخط
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            cell.SetStyle(style);

            // التحقق من توافق تنسيق الخط
            if (fontFormat == FontFileFormatType.Ttf)
            {
                Console.WriteLine("Using TrueType font format");
            }

            // احفظ المصنف
            workbook.Save("FontFileFormatTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


