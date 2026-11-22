---
title: "PivotTable.AllowMultipleFiltersPerField"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. تحدد قيمة منطقية تشير إلى ما إذا كان بإمكان حقول PivotTable أن تحتوي على فلاتر متعددة مُعينة عليها"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/allowmultiplefiltersperfield/
---
## PivotTable.AllowMultipleFiltersPerField property

يحدد قيمة منطقية تشير إلى ما إذا كانت حقول PivotTable يمكن أن تحتوي على فلاتر متعددة مضبوطة عليها.

```csharp
public bool AllowMultipleFiltersPerField { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyAllowMultipleFiltersPerFieldDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 5;
            cells["A6"].Value = "Orange";
            cells["B6"].Value = 10;

            // إنشاء جدول محوري
            int index = sheet.PivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // إضافة حقول إلى جدول محوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // تعيين خاصية AllowMultipleFiltersPerField
            pivotTable.AllowMultipleFiltersPerField = true;
            Console.WriteLine("AllowMultipleFiltersPerField: " + pivotTable.AllowMultipleFiltersPerField);

            // احفظ المصنف
            workbook.Save("PivotTable_AllowMultipleFiltersPerField.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


