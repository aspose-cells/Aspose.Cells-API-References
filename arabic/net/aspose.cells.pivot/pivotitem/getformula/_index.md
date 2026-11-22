---
title: "PivotItem.GetFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotItem. يحصل على صيغة هذا العنصر المحسوب. يعمل فقط عندما يكون هذا العنصر عنصرًا محسوبًا"
type: docs
url: /ar/net/aspose.cells.pivot/pivotitem/getformula/
---
## PivotItem.GetFormula method

يحصل على صيغة هذا العنصر المحسوب. يعمل فقط عندما يكون هذا العنصر عنصرًا محسوبًا.

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
    public class PivotItemMethodGetFormulaDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["B4"].Value = 200;

            // إضافة جدول محوري
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // إضافة حقل الصف وحقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // حساب البيانات
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // احصل على الصيغة من العناصر المحورية
            string rowItemFormula = pivotTable.RowFields[0].PivotItems[0].GetFormula();
            string dataFieldFormula = pivotTable.DataFields[0].GetFormula();

            Console.WriteLine("Row Item Formula: " + rowItemFormula);
            Console.WriteLine("Data Field Formula: " + dataFieldFormula);
        }
    }
}
```

### انظر أيضًا

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


