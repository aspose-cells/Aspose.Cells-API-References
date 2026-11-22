---
title: "Worksheet.IsVisible"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Worksheet property. يمثل ما إذا كانت ورقة العمل مرئية"
type: docs
url: /ar/net/aspose.cells/worksheet/isvisible/
---
## Worksheet.IsVisible property

يمثل ما إذا كانت ورقة العمل مرئية.

```csharp
public bool IsVisible { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة 3 أوراق عمل
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // تعيين ورقة العمل الثانية لتكون مخفية
            workbook.Worksheets[1].IsVisible = false;
            
            // احفظ المصنف
            workbook.Save("WorksheetVisibilityDemo.xlsx");
            
            // عرض حالة الرؤية
            Console.WriteLine("Worksheet Visibility Status:");
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Console.WriteLine($"{workbook.Worksheets[i].Name}: {(workbook.Worksheets[i].IsVisible ? "Visible" : "Hidden")}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


