---
title: "UnionRange.UnMerge"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة UnionRange. تفك دمج الخلايا المدمجة لهذا النطاق"
type: docs
url: /ar/net/aspose.cells/unionrange/unmerge/
---
## UnionRange.UnMerge method

يفك دمج الخلايا المدمجة في هذا النطاق.

```csharp
public void UnMerge()
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodUnMergeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أنشئ نطاقًا ودمج الخلايا
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B2");
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { range });
            
            // ادمج الخلايا وضع قيمة
            unionRange.Merge();
            unionRange.PutValue("Merged Cells", true, true);
            
            try
            {
                // استدعِ طريقة UnMerge
                unionRange.UnMerge();
                
                Console.WriteLine("Cells unmerged successfully");
                
                // ضع قيمًا في الخلايا غير المدمجة لتوضيح التأثير
                worksheet.Cells["A1"].PutValue("A1");
                worksheet.Cells["A2"].PutValue("A2");
                worksheet.Cells["B1"].PutValue("B1");
                worksheet.Cells["B2"].PutValue("B2");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UnMerge method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("MethodUnMergeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


