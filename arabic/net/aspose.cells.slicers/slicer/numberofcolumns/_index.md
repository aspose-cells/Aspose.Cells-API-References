---
title: "Slicer.NumberOfColumns"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Slicer. تُرجع أو تُعيّن عدد الأعمدة في الـ slicer. القيمة الافتراضية هي 1"
type: docs
url: /ar/net/aspose.cells.slicers/slicer/numberofcolumns/
---
## Slicer.NumberOfColumns property

إرجاع أو تعيين عدد الأعمدة في المقطع. القيمة الافتراضية هي 1.

```csharp
public int NumberOfColumns { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerPropertyNumberOfColumnsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // إنشاء بيانات عينة لجدول محوري
            cells["A1"].Value = "Category";
            cells["B1"].Value = "Product";
            cells["A2"].Value = "Fruits";
            cells["B2"].Value = "Apple";
            cells["A3"].Value = "Fruits";
            cells["B3"].Value = "Banana";
            cells["A4"].Value = "Vegetables";
            cells["B4"].Value = "Carrot";

            // إنشاء PivotTable - تخزين الفهرس ثم الحصول على كائن PivotTable
            int pivotIndex = sheet.PivotTables.Add("D1", "A1:B4", "PivotTable");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Product");
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // إضافة slicer متصل بـ PivotTable
            int slicerIndex = sheet.Slicers.Add(pivotTable, "Category", "Slicer1");
            Slicer slicer = sheet.Slicers[slicerIndex];

            // تكوين خصائص slicer
            slicer.Caption = "Product Categories";
            slicer.TopPixel = 50;
            slicer.LeftPixel = 50;
            slicer.HeightPixel = 150;
            slicer.WidthPixel = 200;

            // عرض خاصية NumberOfColumns
            slicer.NumberOfColumns = 2;

            // احفظ المصنف
            workbook.Save("SlicerDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


