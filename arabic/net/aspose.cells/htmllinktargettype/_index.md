---
title: "التعداد HtmlLinkTargetType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.HtmlLinkTargetType. يمثل نوع سمة الهدف في علامة HTML"
type: docs
url: /ar/net/aspose.cells/htmllinktargettype/
---
## HtmlLinkTargetType enumeration

يمثل نوع سمة الهدف في وسم HTML.

```csharp
public enum HtmlLinkTargetType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Blank | `0` | يفتح المستند المرتبط في نافذة أو علامة تبويب جديدة |
| Parent | `1` | يفتح المستند المرتبط في الإطار الأب |
| Self | `2` | يفتح المستند المرتبط في نفس الإطار الذي تم النقر عليه (هذا هو الافتراضي) |
| Top | `3` | يفتح المستند المرتبط في كامل جسم النافذة |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlLinkTargetTypeDemo
    {
        public static void HtmlLinkTargetTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Click here to visit Aspose");
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");

            // إنشاء HtmlSaveOptions وتعيين LinkTargetType
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.LinkTargetType = HtmlLinkTargetType.Blank; // Opens the link in a new window or tab

            // حفظ المصنف بتنسيق HTML
            workbook.Save("HtmlLinkTargetTypeExample.html", saveOptions);

            Console.WriteLine("HTML file saved with link target type set to '_blank'.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


