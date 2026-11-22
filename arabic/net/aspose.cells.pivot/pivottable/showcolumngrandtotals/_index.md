---
title: "PivotTable.ShowColumnGrandTotals"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. تشير إلى ما إذا كان يجب إظهار الإجماليات العامة للأعمدة في جدول المحور هذا"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/showcolumngrandtotals/
---
## PivotTable.ShowColumnGrandTotals property

يشير إلى ما إذا كان يجب إظهار الإجماليات العامة للأعمدة في جدول المحور هذا.

```csharp
public bool ShowColumnGrandTotals { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowColumnGrandTotalsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            var cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["A5"].Value = "Apple";
            cells["B2"].Value = 5;
            cells["B3"].Value = 3;
            cells["B4"].Value = 6;
            cells["B5"].Value = 2;

            // إضافة جدول محوري
            int index = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // تكوين جدول محوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit as rows
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sum of Quantity

            // عرض خاصية ShowColumnGrandTotals
            pivotTable.ShowColumnGrandTotals = false; // Disable column grand totals
            Console.WriteLine("Column Grand Totals Visible: " + pivotTable.ShowColumnGrandTotals);

            // احفظ المصنف
            workbook.Save("PivotTableShowColumnGrandTotalsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


