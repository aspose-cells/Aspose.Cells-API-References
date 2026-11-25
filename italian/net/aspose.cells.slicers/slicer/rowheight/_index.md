---
title: "Slicer.RowHeight"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Slicer. Restituisce o imposta l'altezza di ogni riga nello slicer specificato in unità di punti"
type: docs
url: /it/net/aspose.cells.slicers/slicer/rowheight/
---
## Slicer.RowHeight property

Restituisce o imposta l'altezza di ogni riga nello slicer specificato in unità di punti.

```csharp
public double RowHeight { get; set; }
```

### Esempi

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

### Vedi anche

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


