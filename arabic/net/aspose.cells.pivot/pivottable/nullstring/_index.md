---
title: "PivotTable.NullString"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. تحصل على السلسلة المعروضة في الخلايا التي تحتوي على قيم فارغة عندما تكون الخاصية DisplayNullString صحيحة. القيمة الافتراضية هي سلسلة فارغة"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/nullstring/
---
## PivotTable.NullString property

يحصل على السلسلة المعروضة في الخلايا التي تحتوي على قيم فارغة عندما تكون خاصية DisplayNullString صحيحة. القيمة الافتراضية هي سلسلة فارغة.

```csharp
public string NullString { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyNullStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 3000;
            cells["A5"].Value = null; // Null value
            cells["B5"].Value = 4000;

            // إنشاء جدول محوري
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // إضافة حقول إلى جدول محوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // تعيين خاصية NullString وإعدادات العرض
            pivotTable.NullString = "(null)";
            pivotTable.DisplayNullString = true;

            // تحديث بيانات جدول المحور
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // احفظ المصنف
            workbook.Save("PivotTableNullStringDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


