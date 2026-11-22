---
title: "PivotTable.Indent"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "PivotTable property. تحدد زيادة المسافة البادئة للمحور المدمج ويمكن استخدامها لتعيين تخطيط التقرير إلى الشكل المدمج"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/indent/
---
## PivotTable.Indent property

يحدد زيادة المسافة البادئة للمحور المدمج ويمكن استخدامه لتعيين تخطيط التقرير إلى الشكل المدمج.

```csharp
public int Indent { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyIndentDemo
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
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;

            // إنشاء جدول محوري
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // تعيين خاصية المسافة البادئة
            pivotTable.Indent = 3;
            Console.WriteLine("Pivot Table Indent: " + pivotTable.Indent);

            // احفظ المصنف
            workbook.Save("PivotTableIndentDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


