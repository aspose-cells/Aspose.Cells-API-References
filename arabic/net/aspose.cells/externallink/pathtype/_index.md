---
title: "ExternalLink.PathType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExternalLink. احصل على نوع المسار لهذا الارتباط الخارجي"
type: docs
url: /ar/net/aspose.cells/externallink/pathtype/
---
## ExternalLink.PathType property

احصل على نوع المسار لهذا الارتباط الخارجي

```csharp
public string PathType { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyPathTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أضف ورقة عمل
            Worksheet sheet = workbook.Worksheets[0];
            
            // إنشاء ارتباط خارجي إلى مصنف آخر
            sheet.Cells["A1"].Formula = "='C:\\Temp\\ExternalWorkbook.xlsx'!Sheet1!A1";
            
            // احصل على الارتباط الخارجي
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];
            
            // عرض نوع مسار الارتباط الخارجي
            Console.WriteLine("Path Type: " + externalLink.PathType);
            
            // احفظ المصنف
            workbook.Save("ExternalLinkDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


