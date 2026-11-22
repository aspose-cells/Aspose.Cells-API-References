---
title: "Worksheet.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. تمثل نوع ورقة العمل"
type: docs
url: /ar/net/aspose.cells/worksheet/type/
---
## Worksheet.Type property

يمثل نوع ورقة العمل.

```csharp
public SheetType Type { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين بعض الخصائص الأساسية
            worksheet.Name = "DemoSheet";
            worksheet.IsVisible = true;
            
            // توضيح استخدام خاصية Type
            Console.WriteLine("Worksheet Type: " + worksheet.Type);
            
            // أضف ورقة مخطط لتوضيح نوع ورقة العمل المختلف
            workbook.Worksheets.Add(SheetType.Chart);
            Worksheet chartSheet = workbook.Worksheets[1];
            
            // قارن أنواع ورقة العمل
            Console.WriteLine("Regular Sheet Type: " + worksheet.Type);
            Console.WriteLine("Chart Sheet Type: " + chartSheet.Type);
            
            // احفظ المصنف
            workbook.Save("WorksheetTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [SheetType](../../sheettype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


