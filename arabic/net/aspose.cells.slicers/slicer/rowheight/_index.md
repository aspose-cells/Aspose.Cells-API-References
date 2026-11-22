---
title: "Slicer.RowHeight"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Slicer. تُرجع أو تُعيّن ارتفاع كل صف في المُقَطِّع المحدد بوحدة النقاط"
type: docs
url: /ar/net/aspose.cells.slicers/slicer/rowheight/
---
## Slicer.RowHeight property

يعيد أو يضبط ارتفاع كل صف في المحدد المحدد بوحدة النقاط.

```csharp
public double RowHeight { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerPropertyRowHeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Fruit";
            worksheet.Cells["A3"].Value = "Fruit";
            worksheet.Cells["A4"].Value = "Vegetable";
            
            int pivotIndex = worksheet.PivotTables.Add("A1:A4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "E1", 0);
            Slicer slicer = worksheet.Slicers[slicerIndex];
            
            slicer.RowHeight = 20;
            
            workbook.Save("SlicerRowHeightDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


