---
title: "PivotTable.ConditionalFormats"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. تحصل على التنسيقات الشرطية لجدول المحور"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/conditionalformats/
---
## PivotTable.ConditionalFormats property

يحصل على التنسيقات الشرطية لجدول Pivot.

```csharp
public PivotConditionalFormatCollection ConditionalFormats { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyConditionalFormatsDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 120;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 85;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 95;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 110;

            // إنشاء جدول محوري
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // إضافة صفوف وحقول بيانات
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // إضافة تنسيق شرطي
            int formatIndex = pivotTable.ConditionalFormats.Add();
            PivotConditionalFormat pcf = pivotTable.ConditionalFormats[formatIndex];
            pcf.AddFieldArea(PivotFieldType.Data, pivotTable.DataFields[0]);
            
            // إضافة شرط تنسيق
            int conditionIndex = pcf.FormatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition condition = pcf.FormatConditions[conditionIndex];
            condition.Operator = OperatorType.GreaterOrEqual;
            condition.Formula1 = "100";
            condition.Style.BackgroundColor = Color.Red;

            // احفظ دفتر العمل
            workbook.Save("PivotTableConditionalFormatting.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotConditionalFormatCollection](../../pivotconditionalformatcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


