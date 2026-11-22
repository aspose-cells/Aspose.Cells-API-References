---
title: "HyperlinkCollection.RemoveAt"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة HyperlinkCollection. إزالة الارتباط التشعبي عند الفهرس المحدد في هذه المجموعة"
type: docs
url: /ar/net/aspose.cells/hyperlinkcollection/removeat/
---
## HyperlinkCollection.RemoveAt method

إزالة الارتباط التشعبي عند الفهرس المحدد في هذه المجموعة.

```csharp
public void RemoveAt(int index)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | Int32 | الفهرس الذي يبدأ من الصفر للعنصر. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة ارتباط تشعبي إلى الخلية A1
            sheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // تحقق من وجود الارتباط التشعبي قبل الإزالة
            Console.WriteLine("Hyperlinks count before removal: " + sheet.Hyperlinks.Count);
            
            // إزالة الارتباط التشعبي عند الفهرس 0
            sheet.Hyperlinks.RemoveAt(0);
            
            // تحقق من أنه تم إزالة الارتباط التشعبي
            Console.WriteLine("Hyperlinks count after removal: " + sheet.Hyperlinks.Count);
        }
    }
}
```

### انظر أيضًا

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


