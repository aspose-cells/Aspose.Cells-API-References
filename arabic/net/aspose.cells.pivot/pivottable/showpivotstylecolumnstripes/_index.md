---
title: "PivotTable.ShowPivotStyleColumnStripes"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. تشير إلى ما إذا كان تنسيق الشرائط مطبقًا للعمود"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/showpivotstylecolumnstripes/
---
## PivotTable.ShowPivotStyleColumnStripes property

يشير إلى ما إذا تم تطبيق تنسيق الشرائط للعمود.

```csharp
public bool ShowPivotStyleColumnStripes { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowPivotStyleColumnStripesDemo
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
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 5;
            cells["A6"].Value = "Orange";
            cells["B6"].Value = 12;
            
            // إنشاء جدول محوري
            int index = sheet.PivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // تكوين جدول محوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sum of Quantity
            
            // تمكين شرائط الأعمدة
            pivotTable.ShowPivotStyleColumnStripes = true;
            
            // احفظ المصنف
            workbook.Save("PivotTableColumnStripesDemo.xlsx");
            
            Console.WriteLine("Pivot table with column stripes created successfully.");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


