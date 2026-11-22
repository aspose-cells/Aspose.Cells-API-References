---
title: "التعداد JsonExportHyperlinkType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Json.JsonExportHyperlinkType. يمثل النوع الذي يتم به تصدير الروابط التشعبية إلى json"
type: docs
url: /ar/net/aspose.cells.json/jsonexporthyperlinktype/
---
## JsonExportHyperlinkType enumeration

يمثل نوع طريقة تصدير الروابط التشعبية إلى JSON.

```csharp
public enum JsonExportHyperlinkType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| DisplayString | `0` | تصدير سلسلة العرض |
| Address | `1` | تصدير عنوان URL |
| HtmlString | `2` | تصدير كسلسلة HTML. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Json;
    using System;

    public class JsonExportHyperlinkTypeDemo
    {
        public static void JsonExportHyperlinkTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات النموذجية مع الروابط التشعبية
            worksheet.Cells["A1"].PutValue("Google");
            worksheet.Hyperlinks.Add("A1", 1, 1, "http://www.google.com");

            worksheet.Cells["A2"].PutValue("Aspose");
            worksheet.Hyperlinks.Add("A2", 1, 1, "http://www.aspose.com");

            // إنشاء JsonSaveOptions وتعيين ExportHyperlinkType
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.DisplayString;

            // حفظ المصنف بتنسيق JSON
            workbook.Save("JsonExportHyperlinkTypeExample_HyperlinksDisplayString.json", saveOptions);

            // غيّر ExportHyperlinkType إلى Address واحفظ مرة أخرى
            saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.Address;
            workbook.Save("JsonExportHyperlinkTypeExample_HyperlinksAddress.json", saveOptions);

            // غيّر ExportHyperlinkType إلى HtmlString واحفظ مرة أخرى
            saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.HtmlString;
            workbook.Save("JsonExportHyperlinkTypeExample_HyperlinksHtmlString.json", saveOptions);

            Console.WriteLine("Workbooks saved with different hyperlink export types.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Json](../../aspose.cells.json/)
* assembly [Aspose.Cells](../../)


