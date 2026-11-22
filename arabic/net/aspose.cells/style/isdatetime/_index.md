---
title: "Style.IsDateTime"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Style. تشير إلى ما إذا كان تنسيق الرقم هو تنسيق تاريخ"
type: docs
url: /ar/net/aspose.cells/style/isdatetime/
---
## Style.IsDateTime property

يشير إلى ما إذا كان تنسيق الرقم هو تنسيق تاريخ.

```csharp
public bool IsDateTime { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsDateTimeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // تعيين قيمة رقمية
            cells["A1"].PutValue(1230);
            
            // الحصول على نمط الخلية وتعديله
            Style style = cells["A1"].GetStyle();
            
            // تعيين إلى تنسيق تاريخ (15 هو تنسيق التاريخ المدمج)
            style.Number = 15;
            Console.WriteLine("IsDateTime after setting Number=15: " + style.IsDateTime);
            
            // تعيين تنسيق تاريخ مخصص
            style.Custom = "yyyy-mm-dd";
            Console.WriteLine("IsDateTime after setting custom date format: " + style.IsDateTime);
            
            // تطبيق النمط المعدل مرة أخرى على الخلية
            cells["A1"].SetStyle(style);
        }
    }
}
```

### انظر أيضًا

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


