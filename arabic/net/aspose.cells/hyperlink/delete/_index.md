---
title: "Hyperlink.Delete"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Hyperlink. تحذف هذا الارتباط التشعبي"
type: docs
url: /ar/net/aspose.cells/hyperlink/delete/
---
## Hyperlink.Delete method

يحذف هذا الرابط التشعبي

```csharp
public void Delete()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkMethodDeleteDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بعض الارتباطات التشعبية لتوضيح الحذف
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            worksheet.Hyperlinks.Add("B2", 1, 1, "https://www.example.com");
            
            Console.WriteLine($"Hyperlinks count before deletion: {worksheet.Hyperlinks.Count}");
            
            // احذف جميع الارتباطات التشعبية
            for (int i = worksheet.Hyperlinks.Count - 1; i >= 0; i--)
            {
                worksheet.Hyperlinks[i].Delete();
            }
            
            Console.WriteLine($"Hyperlinks count after deletion: {worksheet.Hyperlinks.Count}");
        }
    }
}
```

### انظر أيضًا

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


