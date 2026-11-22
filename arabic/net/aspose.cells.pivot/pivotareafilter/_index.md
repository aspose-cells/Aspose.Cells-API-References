---
title: "الفئة PivotAreaFilter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Pivot.PivotAreaFilter فئة. يمثل مرشح PivotArea لجدول PivotTable"
type: docs
url: /ar/net/aspose.cells.pivot/pivotareafilter/
---
## PivotAreaFilter class

يمثل مرشح [`PivotArea`](../pivotarea/) لـ [`PivotTable`](../pivottable/).

```csharp
public class PivotAreaFilter
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [PivotAreaFilter](pivotareafilter/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [FieldIndex](../../aspose.cells.pivot/pivotareafilter/fieldindex/) { get; } | يحصل على فهرس الحقل في الحقول المصدر التي يشير إليها هذا المرشح. القيمة -2 تشير إلى حقل القيم. |
| [Selected](../../aspose.cells.pivot/pivotareafilter/selected/) { get; set; } | يشير إلى ما إذا كان لهذا الحقل اختيار. يعمل فقط عندما يكون PivotTable في عرض المخطط التفصيلي. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [IsSubtotalSet](../../aspose.cells.pivot/pivotareafilter/issubtotalset/)(PivotFieldSubtotalType) | يحصل على أي مجموع فرعي تم تعيينه لهذا المرشح. |
| [SetSubtotals](../../aspose.cells.pivot/pivotareafilter/setsubtotals/)(PivotFieldSubtotalType, bool) | المجموع الفرعي للمرشح. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotClassPivotAreaFilterDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إعداد بيانات العينة
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["A3"].Value = "Car";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            
            // إنشاء PivotTable - إصلاح معالجة قيمة الإرجاع
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // إنشاء وتكوين PivotAreaFilter
            PivotAreaFilter filter = new PivotAreaFilter();
            filter.Selected = true;
            filter.SetSubtotals(PivotFieldSubtotalType.Sum, true);
            
            // عرض الطرق
            bool isSumSet = filter.IsSubtotalSet(PivotFieldSubtotalType.Sum);
            Console.WriteLine($"Sum subtotal visibility set: {isSumSet}");
            
            workbook.Save("PivotAreaFilterDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


