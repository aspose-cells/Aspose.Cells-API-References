---
title: "HtmlSaveOptions.LinkTargetType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. تشير إلى نوع سمة الهدف في رابط. القيمة الافتراضية هي HtmlLinkTargetType.Parent"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/linktargettype/
---
## HtmlSaveOptions.LinkTargetType property

يشير إلى نوع خاصية target في رابط `<a>`. القيمة الافتراضية هي HtmlLinkTargetType.Parent.

```csharp
public HtmlLinkTargetType LinkTargetType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyLinkTargetTypeDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Link to Google");
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.google.com");

            // تعيين خيارات حفظ HTML باستخدام LinkTargetType
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.LinkTargetType = HtmlLinkTargetType.Blank;

            // حفظ المصنف كملف HTML
            workbook.Save("output.html", saveOptions);
        }
    }
}
```

### انظر أيضًا

* enum [HtmlLinkTargetType](../../htmllinktargettype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


