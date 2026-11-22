---
title: "Worksheet.ActiveCell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. تحصل أو تعيّن الخلية النشطة في ورقة العمل"
type: docs
url: /ar/net/aspose.cells/worksheet/activecell/
---
## Worksheet.ActiveCell property

يحصل أو يعيّن الخلية النشطة في ورقة العمل.

```csharp
public string ActiveCell { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyActiveCellDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // عيّن الخلية النشطة إلى B2
            worksheet.ActiveCell = "B2";
            
            // طباعة عنوان الخلية النشطة
            Console.WriteLine("Active Cell: " + worksheet.ActiveCell);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
            
            // تحميل المصنف المحفوظ للتحقق من الخلية النشطة
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("Loaded Active Cell: " + loadedWorkbook.Worksheets[0].ActiveCell);
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


