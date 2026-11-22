---
title: "Workbook.HasExernalLinks"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. تشير إلى ما إذا كان هذا المصنف يحتوي على روابط خارجية إلى مصادر بيانات أخرى"
type: docs
url: /ar/net/aspose.cells/workbook/hasexernallinks/
---
## Workbook.HasExernalLinks method

تشير إلى ما إذا كان هذا المصنف يحتوي على روابط خارجية إلى مصادر بيانات أخرى.

```csharp
[Obsolete("Use ExternalLinkCollection.Count property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool HasExernalLinks()
```

### قيمة الإرجاع

ما إذا كان هذا المصنف يحتوي على روابط خارجية إلى مصادر بيانات أخرى.

### ملاحظات

ملاحظة: هذا العضو أصبح الآن غير مستخدم. بدلاً من ذلك، يرجى استخدام ExternalLinkCollection.Count للتحقق مما إذا كانت هناك روابط خارجية في هذا المصنف. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ ديسمبر 2021. تُعتذر شركة Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodHasExernalLinksDemo
    {
        public static void Run()
        {
            // إنشاء مصنف يحتوي على روابط خارجية
            var workbook = new Workbook();
            var worksheet = workbook.Worksheets[0];
            
            // إضافة رابط خارجي
            worksheet.Cells["A1"].Formula = "='http://example.com/[external.xlsx]Sheet1'!A1";
            
            // تحقق مما إذا كان المصنف يحتوي على روابط خارجية
            if (workbook.HasExernalLinks())
            {
                Console.WriteLine("Workbook contains external links:");
                foreach (ExternalLink link in workbook.Worksheets.ExternalLinks)
                {
                    Console.WriteLine($"External Link: {link.DataSource}");
                }
            }
            else
            {
                Console.WriteLine("Workbook has no external links");
            }
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


