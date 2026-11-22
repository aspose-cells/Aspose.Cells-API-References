---
title: "Slicer.LockedPosition"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Slicer. تشير إلى ما إذا كان يمكن نقل الـ Slicer المحدد أو تغيير حجمه باستخدام واجهة المستخدم"
type: docs
url: /ar/net/aspose.cells.slicers/slicer/lockedposition/
---
## Slicer.LockedPosition property

يوضح ما إذا كان يمكن نقل المقطع المحدد أو تغيير حجمه باستخدام واجهة المستخدم.

```csharp
public bool LockedPosition { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyLockedPositionDemo
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
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["B4"].Value = 200;

            // إنشاء مجموعة جداول محورية
            PivotTableCollection pivotTables = worksheet.PivotTables;
            
            // إنشاء جدول محوري
            int pivotIndex = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // إضافة حقل الصف
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");

            // إضافة حقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // إنشاء مجموعة Slicer
            SlicerCollection slicers = worksheet.Slicers;
            
            // إضافة Slicer لجدول المحور
            int slicerIndex = slicers.Add(pivotTable, "A1", "Fruit");
            Slicer slicer = slicers[slicerIndex];

            // تعيين خصائص المحدد
            slicer.Caption = "Fruit Slicer";
            slicer.NumberOfColumns = 2;
            slicer.WidthPixel = 200;
            slicer.HeightPixel = 150;

            // عرض خاصية LockedPosition
            slicer.LockedPosition = true; // Lock the slicer position
            Console.WriteLine("Slicer position locked: " + slicer.LockedPosition);

            // تغيير LockedPosition إلى false للسماح بالحركة
            slicer.LockedPosition = false;
            Console.WriteLine("Slicer position locked: " + slicer.LockedPosition);

            // احفظ المصنف
            workbook.Save("SlicerLockedPositionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


