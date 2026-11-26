---
title: "Slicer.RowHeight"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Slicer. Возвращает или задает высоту каждой строки в указанном срезе в единицах точек"
type: docs
url: /ru/net/aspose.cells.slicers/slicer/rowheight/
---
## Slicer.RowHeight property

Возвращает или задает высоту каждой строки в указанном слайсере в единицах точек.

```csharp
public double RowHeight { get; set; }
```

### Примеры

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

### См. также

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


