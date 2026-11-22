---
title: "PivotArea.RuleType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotArea. تحصل وتعيّن نوع قاعدة الاختيار"
type: docs
url: /ar/net/aspose.cells.pivot/pivotarea/ruletype/
---
## PivotArea.RuleType property

يحصل على نوع قاعدة الاختيار ويضبطه.

```csharp
public PivotAreaType RuleType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyRuleTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Car";
            worksheet.Cells["B3"].Value = 2500;

            // إنشاء جدول محوري مصحّح
            int pivotIndex = worksheet.PivotTables.Add("E5", "A1:B3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivotTable.CalculateData();

            int formatIndex = pivotTable.ConditionalFormats.Add();
            PivotConditionalFormat pfc = pivotTable.ConditionalFormats[formatIndex];
            pfc.AddCellArea(CellArea.CreateCellArea("E5", "F6"));

            Console.WriteLine("PivotArea[0] RuleType: " + pfc.PivotAreas[0].RuleType);
            Console.WriteLine("PivotArea[1] RuleType: " + pfc.PivotAreas[1].RuleType);

            workbook.Save("PivotAreaPropertyRuleTypeDemo_output.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [PivotAreaType](../../pivotareatype/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


