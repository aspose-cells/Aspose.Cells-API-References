---
title: "PivotTableCalculateOption.RefreshData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTableCalculateOption. تشير إلى ما إذا كان يتم تحديث مصدر البيانات للجدول المحوري"
type: docs
url: /ar/net/aspose.cells.pivot/pivottablecalculateoption/refreshdata/
---
## PivotTableCalculateOption.RefreshData property

يشير إلى ما إذا كان تحديث مصدر البيانات لجدول المحور.

```csharp
public bool RefreshData { get; set; }
```

### ملاحظات

إذا كان صحيحًا، قم بتحديث مخزن مؤقت للجدول المحوري من مصدر البيانات، ثم احسب جميع الجداول المحورية بناءً على نفس المخزن المؤقت.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCalculateOptionPropertyRefreshDataDemo
    {
        public static void Run()
        {
            // إنشاء مصنف من ملف Excel المصدر
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إعداد بيانات عينة للجدول المحوري
            var cells = sheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Sales");
            cells["A2"].PutValue("A");
            cells["B2"].PutValue(100);
            cells["A3"].PutValue("B");
            cells["B3"].PutValue(200);
            cells["A4"].PutValue("C");
            cells["B4"].PutValue(300);

            // إنشاء جدول محوري
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // تعديل بيانات المصدر
            cells["B2"].PutValue(150); // Change value from 100 to 150

            // احسب الجدول المحوري باستخدام خيار RefreshData
            PivotTableCalculateOption options = new PivotTableCalculateOption();
            options.RefreshData = true;
            pivotTable.CalculateData(options);

            // إخراج قيمة الجدول المحوري المحدثة
            Console.WriteLine("Updated Pivot Table Value: " + cells["F5"].StringValue);
        }
    }
}
```

### انظر أيضًا

* class [PivotTableCalculateOption](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


