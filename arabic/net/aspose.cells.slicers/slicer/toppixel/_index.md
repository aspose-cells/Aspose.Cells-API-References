---
title: "Slicer.TopPixel"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Slicer. تُعيد أو تُعيّن الإزاحة العمودية لشكل الـ slicer من صفه العلوي بالبكسل"
type: docs
url: /ar/net/aspose.cells.slicers/slicer/toppixel/
---
## Slicer.TopPixel property

تُعيد أو تُعيّن الإزاحة العمودية لشكل الـ slicer من صفه العلوي، بالبكسل.

```csharp
[Obsolete("Use Shape.Top property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int TopPixel { get; set; }
```

### ملاحظات

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام خاصية Shape.Top. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مايو 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerPropertyTopPixelDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // إنشاء بيانات نموذجية
            sheet.Cells["A1"].Value = "Product";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 100;
            sheet.Cells["B3"].Value = 200;
            sheet.Cells["B4"].Value = 300;

            // إنشاء جدول محوري والحصول على فهرسه
            int pivotIndex = sheet.PivotTables.Add("=A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // إضافة slicer والحصول على فهرسه
            int slicerIndex = sheet.Slicers.Add(pivotTable, "A6", 0);
            Slicer slicer = sheet.Slicers[slicerIndex];
            
            // تعيين خاصية TopPixel
            slicer.TopPixel = 6;
            
            workbook.Save("SlicerTopPixelDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


