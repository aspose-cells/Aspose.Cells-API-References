---
title: "PivotTable.ShowPivotStyleLastColumn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. تشير إلى ما إذا كان تنسيق العمود مطبقًا"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/showpivotstylelastcolumn/
---
## PivotTable.ShowPivotStyleLastColumn property

يشير إلى ما إذا تم تطبيق تنسيق العمود.

```csharp
public bool ShowPivotStyleLastColumn { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowPivotStyleLastColumnDemo
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
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // إنشاء جدول محوري
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // تعيين نمط الجدول المحوري وإظهار نمط العمود الأخير
            pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium9;
            pivotTable.ShowPivotStyleLastColumn = true;

            // احفظ المصنف
            workbook.Save("PivotTableShowLastColumnStyle.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


