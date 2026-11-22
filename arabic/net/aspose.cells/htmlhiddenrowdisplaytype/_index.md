---
title: "التعداد HtmlHiddenRowDisplayType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.HtmlHiddenRowDisplayType. يمثل نوعين لعرض الصفوف المخفية في HTML"
type: docs
url: /ar/net/aspose.cells/htmlhiddenrowdisplaytype/
---
## HtmlHiddenRowDisplayType enumeration

يمثل نوعين لعرض الصفوف المخفية في HTML.

```csharp
public enum HtmlHiddenRowDisplayType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Hidden | `0` | إخفاء الصفوف المخفية في صفحة HTML. |
| Remove | `1` | إزالة الصفوف المخفية في صفحة HTML. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlHiddenRowDisplayTypeDemo
    {
        public static void HtmlHiddenRowDisplayTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Visible Row");
            worksheet.Cells["A2"].PutValue("Hidden Row");
            worksheet.Cells["A3"].PutValue("Another Visible Row");

            // إخفاء الصف الثاني
            worksheet.Cells.HideRow(1);

            // إنشاء HtmlSaveOptions وتعيين HiddenRowDisplayType
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden; // or HtmlHiddenRowDisplayType.Remove

            // حفظ المصنف بتنسيق HTML
            workbook.Save("HtmlHiddenRowDisplayTypeExample.html", saveOptions);

            Console.WriteLine("Workbook saved as HTML with hidden row display type.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


