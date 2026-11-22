---
title: "Style.IsNumberFormatApplied"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Style. تشير إلى ما إذا كان يجب تطبيق تنسيق الأرقام"
type: docs
url: /ar/net/aspose.cells/style/isnumberformatapplied/
---
## Style.IsNumberFormatApplied property

يشير إلى ما إذا كان يجب تطبيق تنسيق الأرقام.

```csharp
public bool IsNumberFormatApplied { get; set; }
```

### ملاحظات

فقط للنمط المسمى.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsNumberFormatAppliedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء نمط مع تنسيق الأرقام
            Style style = workbook.CreateStyle();
            style.Number = 14; // Format as "m/d/yyyy"
            style.IsNumberFormatApplied = true;
            
            // تطبيق النمط على خلية
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            
            // تحقق من تطبيق تنسيق الأرقام
            Console.WriteLine("IsNumberFormatApplied: " + style.IsNumberFormatApplied);
            Console.WriteLine("Cell value format: " + cell.GetDisplayStyle().Number);
        }
    }
}
```

### انظر أيضًا

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


