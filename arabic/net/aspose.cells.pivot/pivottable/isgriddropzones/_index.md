---
title: "PivotTable.IsGridDropZones"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. تشير إلى ما إذا كان تقرير PivotTable يعرض تخطيط جدول محوري كلاسيكي. يتيح سحب الحقول في الشبكة"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/isgriddropzones/
---
## PivotTable.IsGridDropZones property

يشير إلى ما إذا كان تقرير PivotTable يعرض تخطيط PivotTable الكلاسيكي. (يمكّن سحب الحقول في الشبكة)

```csharp
public bool IsGridDropZones { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyIsGridDropZonesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // إضافة جدول محوري
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // ضبط خاصية IsGridDropZones
            pivotTable.IsGridDropZones = true;
            Console.WriteLine("IsGridDropZones: " + pivotTable.IsGridDropZones);

            // احفظ المصنف
            workbook.Save("PivotTable_IsGridDropZones_Example.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


