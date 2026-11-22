---
title: "PivotArea.AxisType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotArea. تحصل وتعيّن منطقة جدول PivotTable التي تنطبق عليها هذه القاعدة"
type: docs
url: /ar/net/aspose.cells.pivot/pivotarea/axistype/
---
## PivotArea.AxisType property

يحصل ويضبط منطقة PivotTable التي ينطبق عليها هذا القاعدة.

```csharp
public PivotFieldType AxisType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyAxisTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Electronics";
            worksheet.Cells["A3"].Value = "Clothing";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 800;

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // إضافة حقول إلى مناطق pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);  // Sales

            // إنشاء وتكوين PivotArea
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.AxisType = PivotFieldType.Row; // Demonstrate AxisType property
            pivotArea.RuleType = PivotAreaType.Normal;

            // اختر المنطقة المحورية
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.LabelOnly);

            // احفظ المصنف
            workbook.Save("PivotAreaAxisTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


