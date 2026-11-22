---
title: "PivotTable.ErrorString"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. تحصل على السلسلة المعروضة في الخلايا التي تحتوي على أخطاء عندما تكون خاصية DisplayErrorString صحيحة. القيمة الافتراضية هي سلسلة فارغة."
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/errorstring/
---
## PivotTable.ErrorString property

يحصل على السلسلة المعروضة في الخلايا التي تحتوي على أخطاء عندما تكون خاصية DisplayErrorString صحيحة. القيمة الافتراضية هي سلسلة فارغة.

```csharp
public string ErrorString { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyErrorStringDemo
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
            cells["A2"].Value = "Bike";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Car";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Bike";
            cells["B4"].Value = 1500;
            cells["A5"].Value = "Car";
            cells["B5"].Value = 1800;

            // إنشاء جدول محوري
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // تعيين خاصية ErrorString
            pivotTable.ErrorString = "Custom Error";
            pivotTable.DisplayErrorString = true;

            // إضافة حقول إلى جدول محوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // حساب البيانات وتحديث الجدول المحوري
            pivotTable.CalculateData();
            pivotTable.RefreshData();

            // احفظ المصنف
            workbook.Save("PivotTableErrorStringDemo.xlsx");

            Console.WriteLine("PivotTable with ErrorString property set successfully.");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


