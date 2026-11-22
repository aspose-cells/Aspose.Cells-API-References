---
title: "تعداد HtmlVersion"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.HtmlVersion. يحدد إصدار HTML المستخدم عند الحفظ بتنسيقات Html."
type: docs
url: /ar/net/aspose.cells/htmlversion/
---
## HtmlVersion enumeration

يشير إلى نسخة HTML المستخدمة عند الحفظ بتنسيقات HTML.

```csharp
public enum HtmlVersion
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Default | `0` | احفظ المستند وفقًا لتصدير HTML من MS Excel. |
| XHtml | `1` | يحفظ المستند وفقًا لمعيار XHTML 1.0 الانتقالي. |
| Html5 | `2` | يحفظ المستند وفقًا لمعيار HTML 5. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassHtmlVersionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].PutValue("HTML Version Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates HtmlVersion usage");

            // إنشاء خيارات حفظ HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();

            // حدد إصدار HTML إلى HTML5
            saveOptions.HtmlVersion = HtmlVersion.Html5;

            // احفظ المصنف بإصدار HTML5
            workbook.Save("HtmlVersionDemo_Html5.html", saveOptions);

            // غيّر إصدار HTML إلى XHTML
            saveOptions.HtmlVersion = HtmlVersion.XHtml;

            // احفظ المصنف بإصدار XHTML
            workbook.Save("HtmlVersionDemo_XHtml.html", saveOptions);

            // حدد إصدار HTML إلى الافتراضي (متوافق مع MS Excel)
            saveOptions.HtmlVersion = HtmlVersion.Default;

            // احفظ المصنف بالإصدار الافتراضي
            workbook.Save("HtmlVersionDemo_Default.html", saveOptions);
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


