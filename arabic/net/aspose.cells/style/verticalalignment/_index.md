---
title: "Style.VerticalAlignment"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Style. تحصل أو تعيين نوع المحاذاة العمودية للنص في الخلية"
type: docs
url: /ar/net/aspose.cells/style/verticalalignment/
---
## Style.VerticalAlignment property

يحصل أو يضبط نوع المحاذاة العمودية للنص في الخلية.

```csharp
public TextAlignmentType VerticalAlignment { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyVerticalAlignmentDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى الخلية A1
            Cell cell = worksheet.Cells["A1"];
            
            // ضبط قيمة الخلية
            cell.PutValue("Vertical Alignment Demo");
            
            // الوصول إلى نمط الخلية
            Style style = cell.GetStyle();
            
            // تعيين المحاذاة العمودية إلى الأعلى
            style.VerticalAlignment = TextAlignmentType.Top;
            cell.SetStyle(style);
            
            // احفظ المصنف
            workbook.Save("VerticalAlignmentDemo.xlsx");
            
            Console.WriteLine("Vertical alignment set to Top for cell A1.");
        }
    }
}
```

### انظر أيضًا

* enum [TextAlignmentType](../../textalignmenttype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


