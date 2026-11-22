---
title: "PivotConditionalFormat.ScopeType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotConditionalFormat. احصل على نوع النطاق واضبطه لتنسيق الشرط للجدول المحوري"
type: docs
url: /ar/net/aspose.cells.pivot/pivotconditionalformat/scopetype/
---
## PivotConditionalFormat.ScopeType property

احصل على نوع النطاق واضبطه لتنسيق الجدول المحوري الشرطي .

```csharp
public PivotConditionFormatScopeType ScopeType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PivotConditionalFormatPropertyScopeTypeDemo
    {
        public static void Run()
        {
            // إنشاء مصنف مع جدول محوري
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // بيانات عينة لجدول pivot
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B4"].PutValue(300);

            // إنشاء جدول محوري
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // إضافة تنسيق شرطي إلى الجدول المحوري
            int formatIndex = pivotTable.ConditionalFormats.Add();
            PivotConditionalFormat pcf = pivotTable.ConditionalFormats[formatIndex];
            pcf.ScopeType = PivotConditionFormatScopeType.Data;

            // إضافة شرط تنسيق
            FormatConditionCollection fcs = pcf.FormatConditions;
            CellArea area = new CellArea();
            area.StartRow = 4;
            area.EndRow = 6;
            area.StartColumn = 5;
            area.EndColumn = 5;
            int[] conditionIndex = fcs.Add(area, FormatConditionType.CellValue, OperatorType.Between, "100", "200");
            
            // ضبط نمط التنسيق
            FormatCondition fc = fcs[conditionIndex[0]];
            fc.Style.BackgroundColor = Color.Yellow;

            // احفظ المصنف
            wb.Save("PivotConditionalFormatScopeTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [PivotConditionFormatScopeType](../../pivotconditionformatscopetype/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


