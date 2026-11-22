---
title: "تعداد ExternalLinkType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.ExternalLinkType. يمثل نوع الرابط الخارجي"
type: docs
url: /ar/net/aspose.cells/externallinktype/
---
## ExternalLinkType enumeration

يمثل نوع الرابط الخارجي.

```csharp
public enum ExternalLinkType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| DDELink | `0` | يمثل رابط DDE. |
| External | `1` | يمثل رابطًا خارجيًا. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkTypeDemo
    {
        public static void ExternalLinkTypeExample()
        {
            // فتح ملف يحتوي على روابط خارجية
            Workbook workbook = new Workbook("ExternalLinkTypeExample_original.xlsx");

            // الحصول على الرابط الخارجي 
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];

            // عرض نوع الرابط الخارجي
            Console.WriteLine("External Link Type: " + externalLink.Type);

            // تغيير مصدر بيانات الرابط الخارجي
            externalLink.DataSource = "d:\\link.xls";

            // احفظ المصنف
            workbook.Save("ExternalLinkTypeExample.xlsx");
        }
    }

    // تعداد يمثل نوع الرابط الخارجي
    public enum ExternalLinkType
    {
        DDELink = 0, // Represents the DDE link
        External = 1 // Represents external link
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


