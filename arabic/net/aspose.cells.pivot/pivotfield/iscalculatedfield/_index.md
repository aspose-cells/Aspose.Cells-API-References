---
title: "PivotField.IsCalculatedField"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotField. تشير إلى ما إذا كان هذا الحقل المحوري حقلًا محسوبًا"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/iscalculatedfield/
---
## PivotField.IsCalculatedField property

يحدد ما إذا كان هذا الحقل المحوري حقلًا محسوبًا.

```csharp
public bool IsCalculatedField { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsCalculatedFieldDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = 3000;

            // إضافة جدول محوري
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // إضافة حقل محسوب
            pivotTable.AddCalculatedField("Profit", "Sales*0.2", true);

            // تحقق مما إذا كان الحقل حقلًا محسوبًا
            PivotField profitField = pivotTable.BaseFields[pivotTable.BaseFields.Count - 1];
            Console.WriteLine("Is Profit field calculated? " + profitField.IsCalculatedField);

            // احفظ المصنف
            workbook.Save("PivotField_IsCalculatedField_Example.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


