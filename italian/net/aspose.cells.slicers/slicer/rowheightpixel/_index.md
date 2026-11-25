---
title: "Slicer.RowHeightPixel"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Slicer. Restituisce o imposta l'altezza di ogni riga nello slicer specificato in unità di pixel"
type: docs
url: /it/net/aspose.cells.slicers/slicer/rowheightpixel/
---
## Slicer.RowHeightPixel property

Restituisce o imposta l'altezza di ogni riga nello slicer specificato, in unità di pixel.

```csharp
public int RowHeightPixel { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerPropertyRowHeightPixelDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crea dati di esempio per la tabella pivot
            sheet.Cells["A1"].PutValue("Fruit");
            sheet.Cells["B1"].PutValue("Quantity");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["A3"].PutValue("Orange");
            sheet.Cells["B3"].PutValue(30);
            sheet.Cells["A4"].PutValue("Banana");
            sheet.Cells["B4"].PutValue(40);

            // Crea tabella pivot
            int pivotIndex = workbook.Worksheets[0].PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Aggiungi uno slicer e ottieni il riferimento
            int slicerIndex = sheet.Slicers.Add(pivotTable, "A1", "Fruit");
            Slicer slicer = sheet.Slicers[slicerIndex];
            
            // Imposta le proprietà dello slicer
            slicer.RowHeightPixel = 30;
            slicer.Width = 150;

            workbook.Save("SlicerRowHeightDemo_output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


