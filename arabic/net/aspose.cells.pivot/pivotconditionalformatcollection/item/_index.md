---
title: "PivotConditionalFormatCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotConditionalFormatCollection. يحصل على كائن FormatCondition pivot في الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells.pivot/pivotconditionalformatcollection/item/
---
## PivotConditionalFormatCollection indexer

يحصل على كائن pivot FormatCondition عند الفهرس المحدد.

```csharp
public PivotConditionalFormat this[int index] { get; }
```

### قيمة الإرجاع

كائن FormatCondition pivot.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotConditionalFormatCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إنشاء بيانات عينة لجدول محوري
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 120;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 85;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 95;

            // إنشاء جدول محوري
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // إضافة تنسيق شرطي
            int formatIndex = pivotTable.ConditionalFormats.Add();
            PivotConditionalFormat pfc = pivotTable.ConditionalFormats[formatIndex]; // Using Item property
            pfc.AddCellArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 10, EndColumn = 10 });

            // إضافة شرط تنسيق
            int conditionIndex = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition condition = pfc.FormatConditions[conditionIndex];
            condition.Formula1 = "90";
            condition.Operator = OperatorType.GreaterOrEqual;
            condition.Style.BackgroundColor = System.Drawing.Color.LightGreen;

            // احسب جدول المحور واحفظه
            pivotTable.CalculateData();
            workbook.Save("PivotConditionalFormatExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotConditionalFormat](../../pivotconditionalformat/)
* class [PivotConditionalFormatCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


