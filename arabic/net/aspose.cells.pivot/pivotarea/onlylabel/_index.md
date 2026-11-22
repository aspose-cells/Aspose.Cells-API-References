---
title: "PivotArea.OnlyLabel"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotArea. تشير إلى ما إذا كان يتم اختيار تسميات البيانات فقط لتحديد العنصر"
type: docs
url: /ar/net/aspose.cells.pivot/pivotarea/onlylabel/
---
## PivotArea.OnlyLabel property

يشير إلى ما إذا كانت تسميات البيانات فقط لتحديد عنصر ما مختارة.

```csharp
public bool OnlyLabel { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyOnlyLabelDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // بيانات عينة
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // إضافة حقول
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // تكوين منطقة Pivot
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.AxisType = PivotFieldType.Row;
            pivotArea.OnlyLabel = true; // Key property demonstration
            
            // تطبيق الاختيار
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.LabelOnly);

            workbook.Save("PivotAreaOnlyLabelDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


