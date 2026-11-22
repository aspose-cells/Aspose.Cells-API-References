---
title: "Worksheet.ViewType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. يحصل على ويضبط نوع العرض"
type: docs
url: /ar/net/aspose.cells/worksheet/viewtype/
---
## Worksheet.ViewType property

يحصل على ويضبط نوع العرض.

```csharp
public ViewType ViewType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyViewTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // قم بتعيين نوع العرض إلى PageLayoutView وتمكين المسطرة
            worksheet.ViewType = ViewType.PageLayoutView;
            worksheet.IsRulerVisible = true;
            
            // أضف بعض المحتوى التجريبي لتوضيح العرض
            worksheet.Cells["A1"].PutValue("Page Layout View Demo");
            worksheet.Cells["A2"].PutValue("Ruler is visible in this view");
            
            // احفظ المصنف
            workbook.Save("WorksheetViewTypeDemo.xlsx");
            
            Console.WriteLine("Worksheet ViewType demo completed successfully.");
        }
    }
}
```

### انظر أيضًا

* enum [ViewType](../../viewtype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


