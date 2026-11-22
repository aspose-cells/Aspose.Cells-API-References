---
title: "SparklineGroupCollection.ClearSparklineGroups"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SparklineGroupCollection. تمسح مجموعات Sparkline التي تتداخل مع منطقة من الخلايا"
type: docs
url: /ar/net/aspose.cells.charts/sparklinegroupcollection/clearsparklinegroups/
---
## SparklineGroupCollection.ClearSparklineGroups method

يمسح مجموعات الـ sparkline التي تتداخل مع منطقة من الخلايا.

```csharp
public void ClearSparklineGroups(CellArea cellArea)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| cellArea | CellArea | يحدد منطقة الخلايا |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineGroupCollectionMethodClearSparklineGroupsWithCellAreaDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بعض البيانات إلى ورقة العمل
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // حدد CellArea للمخطط الخطي.
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // أضف مجموعة مخطط خطي إلى ورقة العمل.
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);


            try
            {
                // استدعِ طريقة ClearSparklineGroups مع معامل CellArea
                sheet.SparklineGroups.ClearSparklineGroups(ca);
                
                Console.WriteLine("Sparkline groups cleared successfully for the specified cell area.");
                
                // تحقق من عدد مجموعات Sparkline بعد المسح
                Console.WriteLine($"Remaining sparkline groups count: {sheet.SparklineGroups.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearSparklineGroups method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("ClearSparklineGroupsWithCellAreaDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


