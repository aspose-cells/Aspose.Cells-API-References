---
title: "ExternalLink.IsReferred"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExternalLink. تشير إلى ما إذا كان هذا الرابط الخارجي مُشارًا إليه من قبل آخرين"
type: docs
url: /ar/net/aspose.cells/externallink/isreferred/
---
## ExternalLink.IsReferred property

يشير إلى ما إذا كان هذا الارتباط الخارجي مُشارًا إليه من قبل آخرين.

```csharp
public bool IsReferred { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyIsReferredDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا يحتوي على رابط خارجي
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف إشارة إلى رابط خارجي
            worksheet.Cells["A1"].Formula = "='[external.xlsx]Sheet1'!A1";
            
            // تحقق مما إذا كان يتم الإشارة إلى الارتباط الخارجي
            if (workbook.Worksheets.ExternalLinks.Count > 0)
            {
                bool isReferred = workbook.Worksheets.ExternalLinks[0].IsReferred;
                Console.WriteLine("Is external link referred: " + isReferred);
            }
        }
    }
}
```

### انظر أيضًا

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


