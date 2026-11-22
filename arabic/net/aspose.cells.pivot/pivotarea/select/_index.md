---
title: "PivotArea.Select"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotArea. اختر المنطقة مع عوامل التصفية"
type: docs
url: /ar/net/aspose.cells.pivot/pivotarea/select/
---
## PivotArea.Select method

حدد المنطقة باستخدام المرشحات.

```csharp
public void Select(PivotFieldType axisType, int fieldPosition, 
    PivotTableSelectionType selectionType)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| axisType | PivotFieldType | المنطقة في PivotTable التي ينطبق عليها هذه القاعدة. |
| fieldPosition | Int32 | موضع الحقل داخل المحور الذي تنطبق عليه هذه القاعدة. |
| selectionType | PivotTableSelectionType | يحدد ما يمكن تحديده في PivotTable أثناء اختيار منظم. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaMethodSelectWithPivotFieldTypeInt32PivotTableSDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.LabelOnly);

            workbook.Save("PivotAreaSelectDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [PivotFieldType](../../pivotfieldtype/)
* enum [PivotTableSelectionType](../../pivottableselectiontype/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


