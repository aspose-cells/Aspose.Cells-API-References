---
title: "PivotTable.SaveData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. تشير إلى ما إذا كان يتم حفظ بيانات تقرير جدول البيفوت مع المصنف"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/savedata/
---
## PivotTable.SaveData property

يشير إلى ما إذا كانت بيانات تقرير جدول المحور محفوظة مع المصنف.

```csharp
public bool SaveData { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertySaveDataDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
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
            
            // تكوين جدول محوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // عرض خاصية SaveData
            Console.WriteLine("SaveData before setting: " + pivotTable.SaveData);
            pivotTable.SaveData = false; // Disable saving pivot data with file
            Console.WriteLine("SaveData after setting: " + pivotTable.SaveData);
            
            // احفظ المصنف
            workbook.Save("PivotTable_SaveData_Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


