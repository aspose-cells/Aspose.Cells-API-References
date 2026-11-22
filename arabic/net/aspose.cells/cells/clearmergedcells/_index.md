---
title: "Cells.ClearMergedCells"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تمسح جميع النطاقات المدمجة"
type: docs
url: /ar/net/aspose.cells/cells/clearmergedcells/
---
## Cells.ClearMergedCells method

يمسح جميع النطاقات المدمجة.

```csharp
public void ClearMergedCells()
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodClearMergedCellsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء خلايا مدمجة في A1:B2
            worksheet.Cells.Merge(0, 0, 2, 2);
            Console.WriteLine($"Merged areas before clearing: {worksheet.Cells.GetMergedAreas().Length}");

            try
            {
                // مسح جميع الخلايا المدمجة في ورقة العمل
                worksheet.Cells.ClearMergedCells();
                Console.WriteLine("Method executed successfully");
                Console.WriteLine($"Merged areas after clearing: {worksheet.Cells.GetMergedAreas().Length}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearMergedCells method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("ClearMergedCellsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


