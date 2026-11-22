---
title: "PivotFilterCollection.AddTop10Filter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotFilterCollection. تقوم بالفلترة حسب قيم حقل البيانات المحوري"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfiltercollection/addtop10filter/
---
## PivotFilterCollection.AddTop10Filter method

تصفية حسب القيم لحقل pivot للبيانات.

```csharp
public PivotFilter AddTop10Filter(int baseFieldIndex, int valueFieldIndex, PivotFilterType type, 
    bool isTop, int itemCount)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| baseFieldIndex | Int32 | فهرس الحقل في المصدر. |
| valueFieldIndex | Int32 | فهرس حقل البيانات في منطقة البيانات. |
| type | PivotFilterType | نوع تصفية البيانات. يمكن أن يكون فقط Count أو Sum أو Percent. |
| isTop | منطقي | يشير إلى ما إذا كان الفلتر من الأعلى أم من الأسفل |
| itemCount | Int32 | عدد العناصر |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterCollectionMethodAddTop10FilterWithInt32Int32PivotFilterTypeBooleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Fruit";
            worksheet.Cells["A3"].Value = "Vegetable";
            worksheet.Cells["A4"].Value = "Dairy";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 150;
            worksheet.Cells["B3"].Value = 80;
            worksheet.Cells["B4"].Value = 120;

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // إضافة حقل الصف
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            
            // إضافة حقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            try
            {
                // احصل على مجموعة فلاتر المحور
                PivotFilterCollection filters = pivotTable.PivotFilters;
                
                // أضف فلتر Top10 - عرض أعلى عنصرين حسب المبيعات
                PivotFilter filter = filters.AddTop10Filter(
                    baseFieldIndex: 0,          // Category field
                    valueFieldIndex: 1,          // Sales field
                    type: PivotFilterType.Count, // Filter type
                    isTop: true,                 // Show top items
                    itemCount: 2                 // Number of items to show
                );

                Console.WriteLine($"Top10 filter added successfully. Filter type: {filter.FilterType}");
                Console.WriteLine($"Field index: {filter.FieldIndex}, Value field index: {filter.ValueFieldIndex}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding Top10 filter: {ex.Message}");
            }
            
            // احفظ المصنف
            workbook.Save("PivotFilterCollectionMethodAddTop10FilterDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


