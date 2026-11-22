---
title: "PivotArea.IsOutline"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotArea. تشير إلى ما إذا كانت القاعدة تشير إلى منطقة في وضع المخطط"
type: docs
url: /ar/net/aspose.cells.pivot/pivotarea/isoutline/
---
## PivotArea.IsOutline property

يشير إلى ما إذا كانت القاعدة تشير إلى منطقة في وضع المخطط التفصيلي.

```csharp
public bool IsOutline { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyIsOutlineDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // إضافة حقول إلى جدول محوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales

            // إنشاء وتكوين PivotArea
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.IsOutline = false; // Disable outline style
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.DataAndLabel);

            // احفظ المصنف
            workbook.Save("PivotAreaIsOutlineDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


