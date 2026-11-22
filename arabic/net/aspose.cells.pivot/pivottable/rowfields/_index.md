---
title: "PivotTable.RowFields"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. تُرجع مجموعة PivotFieldCollection التي تُعرض حاليًا كحقول صف"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/rowfields/
---
## PivotTable.RowFields property

تُرجع [`PivotFieldCollection`](../../pivotfieldcollection/) التي تُعرض حاليًا كحقول صف.

```csharp
public PivotFieldCollection RowFields { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRowFieldsDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Bike";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            
            cells["A3"].Value = "Bike";
            cells["B3"].Value = "South";
            cells["C3"].Value = 800;
            
            cells["A4"].Value = "Car";
            cells["B4"].Value = "North";
            cells["C4"].Value = 1500;
            
            cells["A5"].Value = "Car";
            cells["B5"].Value = "South";
            cells["C5"].Value = 1200;

            // إنشاء جدول محوري
            int pivotIndex = sheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // إضافة حقول الصف
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Region");
            
            // إضافة حقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // عرض خاصية RowFields
            Console.WriteLine("Row Fields Count: " + pivotTable.RowFields.Count);
            Console.WriteLine("First Row Field Name: " + pivotTable.RowFields[0].Name);
            Console.WriteLine("Second Row Field Name: " + pivotTable.RowFields[1].Name);
            
            // احفظ المصنف
            workbook.Save("PivotTableRowFieldsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


