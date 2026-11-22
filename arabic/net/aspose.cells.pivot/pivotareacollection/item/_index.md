---
title: "PivotAreaCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotAreaCollection. تحصل على كائن PivotArea"
type: docs
url: /ar/net/aspose.cells.pivot/pivotareacollection/item/
---
## PivotAreaCollection indexer

تحصل على كائن [`PivotArea`](../../pivotarea/)؛

```csharp
public PivotArea this[int index] { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PivotAreaCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إنشاء بيانات عينة لجدول محوري
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 100;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 150;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 200;

            // إنشاء جدول محوري
            PivotTableCollection pivotTables = sheet.PivotTables;
            int pivotIndex = pivotTables.Add("A5", "A1:B4", "PivotTable");
            PivotTable pivot = pivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // إضافة تنسيق شرطي
            int formatIndex = pivot.ConditionalFormats.Add();
            PivotConditionalFormat pfc = pivot.ConditionalFormats[formatIndex];
            pfc.AddCellArea(CellArea.CreateCellArea("A5", "B8"));

            // الوصول إلى PivotAreas باستخدام خاصية Item
            PivotArea pivotArea = pfc.PivotAreas[0]; // Using Item indexer
            pivotArea.RuleType = PivotAreaType.All;

            // إضافة شرط تنسيق
            int conditionIndex = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition condition = pfc.FormatConditions[conditionIndex];
            condition.Formula1 = "150";
            condition.Operator = OperatorType.GreaterOrEqual;
            condition.Style.BackgroundColor = Color.Red;

            // احسب واحفظ
            pivot.CalculateData();
            workbook.Save("PivotAreaCollectionPropertyItemDemo_output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotArea](../../pivotarea/)
* class [PivotAreaCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


