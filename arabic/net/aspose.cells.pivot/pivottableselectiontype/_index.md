---
title: "تعداد PivotTableSelectionType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Pivot.PivotTableSelectionType. يحدد ما يمكن تحديده في PivotTable أثناء اختيار منظم. يمكن دمج هذه الثوابت لتحديد أنواع متعددة."
type: docs
url: /ar/net/aspose.cells.pivot/pivottableselectiontype/
---
## PivotTableSelectionType enumeration

يحدد ما يمكن تحديده في جدول PivotTable أثناء اختيار منظم. يمكن دمج هذه الثوابت لتحديد أنواع متعددة.

```csharp
public enum PivotTableSelectionType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| DataAndLabel | `0` | البيانات والتسميات |
| DataOnly | `2` | يختار البيانات فقط |
| LabelOnly | `1` | يختار التسميات فقط |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableSelectionTypeDemo
    {
        public static void PivotTableSelectionTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات إلى PivotTable
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(200);
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B5"].PutValue(250);

            // إنشاء PivotTable
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // إضافة حقول إلى PivotTable
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // إنشاء PivotArea وتعيين خصائصه
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.AxisType = PivotFieldType.Row;
            pivotArea.OnlyData = false;
            pivotArea.OnlyLabel = true;
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.IsColumnGrandIncluded = true;
            pivotArea.IsOutline = false;

            // حدد المنطقة بنوع اختيار محدد
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.LabelOnly);

            // احفظ المصنف
            workbook.Save("PivotTableSelectionTypeExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


