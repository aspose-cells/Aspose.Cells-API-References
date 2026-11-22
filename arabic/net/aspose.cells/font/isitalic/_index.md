---
title: "Font.IsItalic"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية الخط. تحصل أو تعين قيمة تشير إلى ما إذا كان الخط مائل"
type: docs
url: /ar/net/aspose.cells/font/isitalic/
---
## Font.IsItalic property

يحصل على أو يضبط قيمة تشير إلى ما إذا كان الخط مائلًا.

```csharp
public bool IsItalic { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsItalicDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى النمط الافتراضي
            Style style = workbook.DefaultStyle;
            
            // تعيين خصائص الخط بما في ذلك IsItalic
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.Font.IsItalic = true;
            
            // تطبيق النمط على الخلية A1
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Italic Text Example");
            
            // احفظ المصنف
            workbook.Save("FontPropertyIsItalicDemo.xlsx");
            
            // تحقق من خاصية المائل
            Console.WriteLine("Font is italic: " + cell.GetStyle().Font.IsItalic);
        }
    }
}
```

### انظر أيضًا

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


