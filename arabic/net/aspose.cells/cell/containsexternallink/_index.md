---
title: "Cell.ContainsExternalLink"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cell. تشير إلى ما إذا كانت هذه الخلية تحتوي على رابط خارجي. تُطبق فقط عندما تكون الخلية خلية صيغة."
type: docs
url: /ar/net/aspose.cells/cell/containsexternallink/
---
## Cell.ContainsExternalLink property

يشير إلى ما إذا كانت هذه الخلية تحتوي على رابط خارجي. ينطبق فقط عندما تكون الخلية خلية صيغة.

```csharp
public bool ContainsExternalLink { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyContainsExternalLinkDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet sheet = workbook.Worksheets[0];
            
            // أضف بيانات عينة ورابطًا خارجيًا
            sheet.Cells["A1"].PutValue("External Link:");
            sheet.Cells["B1"].Formula = "=HYPERLINK(\"https://www.aspose.com\", \"Aspose\")";
            
            // تحقق مما إذا كانت الخلايا تحتوي على روابط خارجية
            Console.WriteLine("A1 ContainsExternalLink: " + sheet.Cells["A1"].ContainsExternalLink);
            Console.WriteLine("B1 ContainsExternalLink: " + sheet.Cells["B1"].ContainsExternalLink);
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


