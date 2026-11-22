---
title: "PivotTable.PivotFilters"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. تُرجع جميع الفلاتر في جدول المحور"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/pivotfilters/
---
## PivotTable.PivotFilters property

يعيد جميع الفلاتر في جدول PivotTable.

```csharp
public PivotFilterCollection PivotFilters { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyPivotFiltersDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            try
            {
                // إنشاء جدول محوري
                int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // إضافة حقول إلى الجدول المحوري
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

                // الوصول إلى مجموعة PivotFilters (خاصية للقراءة فقط)
                PivotFilterCollection pivotFilters = pivotTable.PivotFilters;

                // عرض المعلومات حول مجموعة PivotFilters
                Console.WriteLine("Number of PivotFilters: " + pivotFilters.Count);

                // التكرار عبر الفلاتر وعرض أنواعها
                for (int i = 0; i < pivotFilters.Count; i++)
                {
                    PivotFilter filter = pivotFilters[i];
                    Console.WriteLine($"Filter {i + 1} Type: {filter.FilterType}");
                }

                // إضافة فلتر تجريبي لتوضيح الوظيفة
                if (pivotFilters.Count == 0)
                {
                    // إضافة فلتر قيمة إلى الحقل الأول (Sales)
                    PivotFilter valueFilter = pivotFilters.AddValueFilter(0, 1,
                        PivotFilterType.ValueGreaterThan, 150.0, 0.0);
                    Console.WriteLine("Added value filter: Greater than 150");
                }

                // عرض عدد الفلاتر المحدث
                Console.WriteLine("Updated number of PivotFilters: " + pivotFilters.Count);

                // احفظ المصنف
                workbook.Save("PivotFiltersDemo.xlsx");
                Console.WriteLine("PivotFilters demonstration completed successfully.");
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

* class [PivotFilterCollection](../../pivotfiltercollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


