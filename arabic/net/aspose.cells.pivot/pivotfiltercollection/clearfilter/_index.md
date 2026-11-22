---
title: "PivotFilterCollection.ClearFilter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotFilterCollection. مسح PivotFilter من PivotField المحدد"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfiltercollection/clearfilter/
---
## PivotFilterCollection.ClearFilter method

مسح PivotFilter من PivotField المحدد

```csharp
public void ClearFilter(int fieldIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldIndex | Int32 | فهرس PivotField |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterCollectionMethodClearFilterWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["B4"].Value = 8;

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // إضافة حقل الصف
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            
            // إضافة حقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // إضافة مرشح إلى الجدول المحوري
            PivotFilterCollection filters = pivotTable.PivotFilters;
            filters.AddLabelFilter(0, PivotFilterType.Count, "Apple", null);

            try
            {
                // استدعاء طريقة ClearFilter مع معامل فهرس الحقل
                filters.ClearFilter(0);
                
                Console.WriteLine("Pivot filter cleared successfully for field index 0");
                
                // تحقق من أن المرشح قد تم مسحه
                Console.WriteLine($"Number of filters after clearing: {filters.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearFilter method: {ex.Message}");
            }
            
            // احفظ المصنف
            workbook.Save("PivotFilterCollectionMethodClearFilterWithInt32Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


