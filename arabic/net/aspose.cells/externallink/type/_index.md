---
title: "ExternalLink.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExternalLink. تحصل على نوع الارتباط الخارجي"
type: docs
url: /ar/net/aspose.cells/externallink/type/
---
## ExternalLink.Type property

يحصل على نوع الارتباط الخارجي.

```csharp
public ExternalLinkType Type { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أضف ورقة عمل
            Worksheet sheet = workbook.Worksheets[0];
            
            // إنشاء ارتباط خارجي إلى مصنف آخر
            sheet.Cells["A1"].Formula = "='[link.xls]Sheet1'!A1";
            
            // احصل على الارتباط الخارجي
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];
            
            // عرض نوع الرابط الخارجي
            Console.WriteLine("External Link Type: " + externalLink.Type);
            
            // تغيير مصدر بيانات الارتباط الخارجي
            externalLink.DataSource = "d:\\link.xls";
            
            // احفظ المصنف
            workbook.Save("ExternalLinkTypeExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ExternalLinkType](../../externallinktype/)
* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


