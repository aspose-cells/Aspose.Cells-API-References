---
title: "WorksheetCollection.ExternalLinks"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorksheetCollection. تمثل الروابط الخارجية في دفتر العمل"
type: docs
url: /ar/net/aspose.cells/worksheetcollection/externallinks/
---
## WorksheetCollection.ExternalLinks property

يمثل الروابط الخارجية في مصنف العمل.

```csharp
public ExternalLinkCollection ExternalLinks { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyExternalLinksDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل مصدر يحتوي على رابط خارجي
            var sourceWorkbook = new Workbook();
            sourceWorkbook.Worksheets.Add("Sheet1");
            sourceWorkbook.Worksheets.ExternalLinks.Add("external.xlsx", new string[] { "Sheet1!A1" });
            
            // إنشاء دفتر عمل هدف
            var destWorkbook = new Workbook();
            destWorkbook.Worksheets.Add("Sheet1");

            // تعيين مصدر بيانات الرابط الخارجي
            Console.WriteLine("Original external link: {0}", sourceWorkbook.Worksheets.ExternalLinks[0].DataSource);
            sourceWorkbook.Worksheets.ExternalLinks[0].DataSource = "updated_external.xlsx";
            Console.WriteLine("Updated external link: {0}", sourceWorkbook.Worksheets.ExternalLinks[0].DataSource);

            // احفظ المصنف
            sourceWorkbook.Save("output.xlsx");
            Console.WriteLine("Workbook saved with updated external link.");

            // تنظيف
            sourceWorkbook.Dispose();
            destWorkbook.Dispose();
        }
    }
}
```

### انظر أيضًا

* class [ExternalLinkCollection](../../externallinkcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


