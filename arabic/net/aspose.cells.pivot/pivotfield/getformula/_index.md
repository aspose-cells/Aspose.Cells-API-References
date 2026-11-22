---
title: "PivotField.GetFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotField. تحصل على صيغة الحقل المحسوب. تعمل فقط مع الحقل المحسوب"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/getformula/
---
## PivotField.GetFormula method

يحصل على صيغة الحقل المحسوب. يعمل فقط مع الحقل المحسوب.

```csharp
public string GetFormula()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodGetFormulaDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Car";
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["A4"].Value = "Bike";
            worksheet.Cells["B4"].Value = 1500;
            
            // إنشاء جدول محوري
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // إضافة حقل محسوب مع صيغة
            pivotTable.AddCalculatedField("=ABS('Sales')", "Absolute Sales");
            
            // الحصول على الصيغة من الحقل المحسوب
            PivotFieldCollection fields = pivotTable.DataFields;
            string formula = fields[fields.Count - 1].GetFormula();
            
            // إخراج الصيغة
            Console.WriteLine("Calculated field formula: " + formula);
        }
    }
}
```

### انظر أيضًا

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


