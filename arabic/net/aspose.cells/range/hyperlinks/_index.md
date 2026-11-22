---
title: "Range.Hyperlinks"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Range. يحصل على جميع الروابط التشعبية في النطاق"
type: docs
url: /ar/net/aspose.cells/range/hyperlinks/
---
## Range.Hyperlinks property

يحصل على جميع الروابط التشعبية في النطاق.

```csharp
public Hyperlink[] Hyperlinks { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyHyperlinksDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة ارتباط تشعبي إلى الخلية A1
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // إنشاء نطاق يحتوي على A1
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1");
            
            // احصل على الروابط التشعبية في النطاق
            Hyperlink[] hyperlinks = range.Hyperlinks;
            
            // عرض معلومات الرابط التشعبي
            if (hyperlinks.Length > 0)
            {
                Console.WriteLine("Hyperlink found:");
                Console.WriteLine($"Address: {hyperlinks[0].Address}");
                Console.WriteLine($"Link Type: {hyperlinks[0].LinkType}");
                
                // حذف الارتباط التشعبي
                hyperlinks[0].Delete();
                Console.WriteLine("Hyperlink deleted");
            }
            
            // تحقق من أنه تم إزالة الارتباط التشعبي
            Console.WriteLine($"Total hyperlinks in worksheet: {worksheet.Hyperlinks.Count}");
        }
    }
}
```

### انظر أيضًا

* class [Hyperlink](../../hyperlink/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


