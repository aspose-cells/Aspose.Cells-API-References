---
title: "Worksheet.IsSelected"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. تشير إلى ما إذا كانت هذه الورقة مختارة عند فتح دفتر العمل"
type: docs
url: /ar/net/aspose.cells/worksheet/isselected/
---
## Worksheet.IsSelected property

يشير إلى ما إذا تم اختيار ورقة العمل هذه عند فتح المصنف.

```csharp
public bool IsSelected { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsSelectedDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة ورقة عمل ثانية
            workbook.Worksheets.Add("Sheet2");
            
            // احصل على ورقة العمل الأولى
            Worksheet worksheet1 = workbook.Worksheets[0];
            worksheet1.Name = "FirstSheet";
            
            // الحصول على ورقة العمل الثانية
            Worksheet worksheet2 = workbook.Worksheets[1];
            worksheet2.Name = "SecondSheet";
            
            // عرض خاصية IsSelected
            Console.WriteLine("Before selection:");
            Console.WriteLine($"Worksheet1 IsSelected: {worksheet1.IsSelected}");
            Console.WriteLine($"Worksheet2 IsSelected: {worksheet2.IsSelected}");
            
            // تحديد ورقة العمل الثانية
            worksheet2.IsSelected = true;
            workbook.Worksheets.ActiveSheetIndex = worksheet2.Index;
            
            Console.WriteLine("\nAfter selection:");
            Console.WriteLine($"Worksheet1 IsSelected: {worksheet1.IsSelected}");
            Console.WriteLine($"Worksheet2 IsSelected: {worksheet2.IsSelected}");
            
            // احفظ المصنف
            workbook.Save("WorksheetSelectionDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


