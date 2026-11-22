---
title: "Spinner.IsHorizontal"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Spinner. تشير إلى ما إذا كان هذا شريط تمرير أفقي"
type: docs
url: /ar/net/aspose.cells.drawing/spinner/ishorizontal/
---
## Spinner.IsHorizontal property

يشير إلى ما إذا كان هذا شريط تمرير أفقي.

```csharp
public bool IsHorizontal { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class SpinnerPropertyIsHorizontalDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // إضافة شكل Spinner إلى ورقة العمل
                Spinner spinner = worksheet.Shapes.AddSpinner(1, 0, 1, 0, 100, 30);
                
                // اضبط خصائص Spinner
                spinner.Min = 0;
                spinner.Max = 100;
                spinner.IncrementalChange = 5;
                spinner.CurrentValue = 50;
                
                // عرض خاصية IsHorizontal (قراءة وكتابة)
                Console.WriteLine("Initial IsHorizontal value: " + spinner.IsHorizontal);
                
                // تبديل الاتجاه
                spinner.IsHorizontal = !spinner.IsHorizontal;
                Console.WriteLine("Modified IsHorizontal value: " + spinner.IsHorizontal);
                
                // احفظ المصنف
                workbook.Save("SpinnerIsHorizontalDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


