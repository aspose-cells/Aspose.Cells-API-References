---
title: "UnionRange.Merge"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة UnionRange. تجمع نطاقًا من الخلايا في خلية واحدة"
type: docs
url: /ar/net/aspose.cells/unionrange/merge/
---
## UnionRange.Merge method

يجمع نطاقًا من الخلايا في خلية واحدة.

```csharp
public void Merge()
```

### ملاحظات

الإشارة إلى الخلية المدمجة عبر عنوان الخلية العليا اليسرى في النطاق.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodMergeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أنشئ نطاقًا من الخلايا (A1:B2)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B2");
            
            // ضع بعض البيانات في الخلايا لتصوّر الدمج
            range[0, 0].PutValue("Before Merge");
            range[0, 1].PutValue("A1");
            range[1, 0].PutValue("B1");
            range[1, 1].PutValue("B2");
            
            try
            {
                // أنشئ UnionRange من النطاق
                UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { range });
                
                // استدعِ طريقة Merge
                unionRange.Merge();
                
                // ضع قيمة في الخلية المدمجة
                unionRange.PutValue("Merged A1:B2", true, true);
                
                Console.WriteLine("Cells merged successfully");
                
                // إلغاء التعليق لرؤية تأثير فك الدمج
                // unionRange.UnMerge();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Merge method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("MethodMergeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


