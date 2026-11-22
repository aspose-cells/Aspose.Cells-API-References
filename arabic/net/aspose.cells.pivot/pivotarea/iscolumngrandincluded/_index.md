---
title: "PivotArea.IsColumnGrandIncluded"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotArea. تشير إلى ما إذا كان إجمالي العمود الكلي مدرجًا"
type: docs
url: /ar/net/aspose.cells.pivot/pivotarea/iscolumngrandincluded/
---
## PivotArea.IsColumnGrandIncluded property

يشير إلى ما إذا كان المجموع الكلي للعمود مشمولًا.

```csharp
public bool IsColumnGrandIncluded { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyIsColumnGrandIncludedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // بيانات عينة
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Fruit";
            worksheet.Cells["A3"].Value = "Vegetable";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 150;

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // إضافة حقول
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // تكوين منطقة Pivot
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.IsColumnGrandIncluded = true; // Demonstrate property usage
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.RuleType = PivotAreaType.Normal;

            // احفظ المصنف
            workbook.Save("PivotAreaIsColumnGrandIncludedDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


