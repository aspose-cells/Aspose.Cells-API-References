---
title: "التعداد HtmlHiddenColDisplayType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.HtmlHiddenColDisplayType. يمثل نوعين لعرض الأعمدة المخفية في HTML"
type: docs
url: /ar/net/aspose.cells/htmlhiddencoldisplaytype/
---
## HtmlHiddenColDisplayType enumeration

يمثل نوعين لعرض الأعمدة المخفية في HTML.

```csharp
public enum HtmlHiddenColDisplayType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Hidden | `0` | إخفاء الأعمدة المخفية في صفحة HTML. |
| Remove | `1` | إزالة الأعمدة المخفية في صفحة HTML. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlHiddenColDisplayTypeDemo
    {
        public static void HtmlHiddenColDisplayTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // إخفاء العمود الثاني
            worksheet.Cells.HideColumn(1);

            // إنشاء HtmlSaveOptions وتعيين HiddenColDisplayType
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.HiddenColDisplayType = HtmlHiddenColDisplayType.Remove;

            // حفظ المصنف بتنسيق HTML
            workbook.Save("HtmlHiddenColDisplayTypeExample.html", saveOptions);

            Console.WriteLine("Workbook saved as HTML with hidden columns removed.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


