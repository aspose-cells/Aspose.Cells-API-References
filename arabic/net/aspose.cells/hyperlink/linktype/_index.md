---
title: "Hyperlink.LinkType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Hyperlink. تحصل على نوع الرابط"
type: docs
url: /ar/net/aspose.cells/hyperlink/linktype/
---
## Hyperlink.LinkType property

يحصل على نوع الارتباط.

```csharp
public TargetModeType LinkType { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkPropertyLinkTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة ارتباط تشعبي خارجي
            int hyperlinkIndex = worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            Hyperlink link = worksheet.Hyperlinks[hyperlinkIndex];
            
            // توضيح خاصية LinkType
            Console.WriteLine("Hyperlink LinkType: " + link.LinkType);
            
            // تنظيف
            link.Delete();
            Console.WriteLine("Hyperlinks count after deletion: " + worksheet.Hyperlinks.Count);
        }
    }
}
```

### انظر أيضًا

* enum [TargetModeType](../../targetmodetype/)
* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


