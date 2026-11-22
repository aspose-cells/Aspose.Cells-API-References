---
title: "ExternalLinkCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExternalLinkCollection. تحصل على عنصر ExternalLink في الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells/externallinkcollection/item/
---
## ExternalLinkCollection indexer

تحصل على العنصر [`ExternalLink`](../../externallink/) في الفهرس المحدد.

```csharp
public ExternalLink this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس الذي يبدأ من الصفر للعنصر. |

### قيمة الإرجاع

العنصر عند الفهرس المحدد.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء مصنف يحتوي على روابط خارجية نموذجية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بعض الروابط الخارجية
            worksheet.Cells["A1"].Formula = "='C:\\Temp\\External1.xlsx'!A1";
            worksheet.Cells["A2"].Formula = "='C:\\Temp\\External2.xlsx'!B2";
            
            // الوصول إلى الروابط الخارجية باستخدام خاصية Item
            for (int i = 0; i < workbook.Worksheets.ExternalLinks.Count; i++)
            {
                ExternalLink link = workbook.Worksheets.ExternalLinks[i];
                Console.WriteLine($"External Link {i + 1}:");
                Console.WriteLine($"- DataSource: {link.DataSource}");
                Console.WriteLine($"- OriginalDataSource: {link.OriginalDataSource}");
            }
        }
    }
}
```

### انظر أيضًا

* class [ExternalLink](../../externallink/)
* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


