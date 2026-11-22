---
title: "Worksheet.IsPageBreakPreview"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. تشير إلى ما إذا كانت ورقة العمل المحددة تُعرض في العرض العادي أو معاينة فواصل الصفحات"
type: docs
url: /ar/net/aspose.cells/worksheet/ispagebreakpreview/
---
## Worksheet.IsPageBreakPreview property

يشير إلى ما إذا كانت ورقة العمل المحددة تُعرض في العرض العادي أو معاينة فواصل الصفحات.

```csharp
public bool IsPageBreakPreview { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsPageBreakPreviewDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // اضبط ورقة العمل على وضع معاينة فواصل الصفحات
            worksheet.IsPageBreakPreview = true;
            
            // اضبط التكبير إلى 100٪ للعرض التوضيحي
            worksheet.Zoom = 100;
            
            // إخراج الإعدادات الحالية
            Console.WriteLine("IsPageBreakPreview: " + worksheet.IsPageBreakPreview);
            Console.WriteLine("Zoom: " + worksheet.Zoom);
            
            // احفظ المصنف
            workbook.Save("WorksheetPropertyIsPageBreakPreviewDemo_output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


