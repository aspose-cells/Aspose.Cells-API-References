---
title: "HtmlLoadOptions.ProgId"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlLoadOptions. تحصل على معرف البرنامج لإنشاء الملف. فقط لملفات MHT"
type: docs
url: /ar/net/aspose.cells/htmlloadoptions/progid/
---
## HtmlLoadOptions.ProgId property

يحصل على معرف البرنامج لإنشاء الملف. ينطبق فقط على ملفات MHT.

```csharp
public string ProgId { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyProgIdDemo
    {
        public static void Run()
        {
            // إنشاء خيارات تحميل HTML بصيغة MHTML
            HtmlLoadOptions options = new HtmlLoadOptions(LoadFormat.MHtml);
            
            // احصل على خاصية ProgId
            Console.WriteLine("ProgId is: " + options.ProgId);

            // إنشاء نسخة أخرى والحصول على ProgId الخاص بها
            HtmlLoadOptions wordOptions = new HtmlLoadOptions(LoadFormat.MHtml);
            Console.WriteLine("ProgId is: " + wordOptions.ProgId);
        }
    }
}
```

### انظر أيضًا

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


