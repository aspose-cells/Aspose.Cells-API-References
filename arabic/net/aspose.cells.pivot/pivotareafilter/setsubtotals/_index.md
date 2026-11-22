---
title: "PivotAreaFilter.SetSubtotals"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotAreaFilter. المجموع الفرعي للمرشح"
type: docs
url: /ar/net/aspose.cells.pivot/pivotareafilter/setsubtotals/
---
## PivotAreaFilter.SetSubtotals method

المجموع الفرعي للمرشح.

```csharp
public void SetSubtotals(PivotFieldSubtotalType subtotalType, bool shown)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| subtotalType | PivotFieldSubtotalType | دالة التجميع الفرعي. |
| معروض | منطقي | يشير إلى ما إذا كان يتم عرض بيانات المجموع الفرعي هذه. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaFilterMethodSetSubtotalsWithPivotFieldSubtotalTypeBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء بيانات عينة لجدول محوري
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 8;

            // إنشاء جدول محوري
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("=A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // إنشاء منطقة محورية باستخدام معامل جدول المحور
            PivotArea pivotArea = new PivotArea(pivotTable);
            PivotAreaFilter filter = new PivotAreaFilter();

            try
            {
                // استدعِ SetSubtotals مع نوع المجموع الفرعي Sum واضبطه للعرض
                filter.SetSubtotals(PivotFieldSubtotalType.Sum, true);
                
                // تحقق مما إذا تم ضبط المجموع الفرعي
                bool isSumSet = filter.IsSubtotalSet(PivotFieldSubtotalType.Sum);
                Console.WriteLine($"Sum subtotal is set: {isSumSet}");

                // قم بتحديث جدول المحور لرؤية التغييرات
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetSubtotals method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("PivotAreaFilterSetSubtotalsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotAreaFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


