---
title: "PivotArea.Filters"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotArea. تحصل على جميع الفلاتر لهذه PivotArea"
type: docs
url: /ar/net/aspose.cells.pivot/pivotarea/filters/
---
## PivotArea.Filters property

يحصل على جميع الفلاتر لهذا PivotArea.

```csharp
public PivotAreaFilterCollection Filters { get; }
```

### أمثلة

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyFiltersDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "SalesData";
            
            // إنشاء بيانات نموذجية
            dataSheet.Cells["A1"].PutValue("Category");
            dataSheet.Cells["B1"].PutValue("Revenue");
            dataSheet.Cells["A2"].PutValue("Electronics");
            dataSheet.Cells["B2"].PutValue(1500);
            dataSheet.Cells["A3"].PutValue("Furniture");
            dataSheet.Cells["B3"].PutValue(800);
            dataSheet.Cells["A4"].PutValue("Electronics");
            dataSheet.Cells["B4"].PutValue(2200);

            // إنشاء جدول محوري
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotReport");
            int pivotIndex = pivotSheet.PivotTables.Add("A3", "SalesData!A1:B4", "RevenueAnalysis");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];

            // تكوين حقل الصف مع المجاميع الفرعية
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pivotTable.RowFields["Category"];
            rowField.IsAutoSubtotals = true;

            // إضافة حقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Revenue");

            // إنشاء PivotArea وتحديد الحقول
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.SelectField(PivotFieldType.Data, "Sum of Revenue");
            pivotArea.SelectField(PivotFieldType.Row, "Category");

            // عرض مثال على استخدام خاصية Filters
            Console.WriteLine($"Filter count: {pivotArea.Filters.Count}");
            if (pivotArea.Filters.Count > 1)
            {
                bool hasAutomaticSubtotal = pivotArea.Filters[1].IsSubtotalSet(PivotFieldSubtotalType.Automatic);
                Console.WriteLine($"Row field has automatic subtotal: {hasAutomaticSubtotal}");
            }

            workbook.Save("PivotFiltersDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotAreaFilterCollection](../../pivotareafiltercollection/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


