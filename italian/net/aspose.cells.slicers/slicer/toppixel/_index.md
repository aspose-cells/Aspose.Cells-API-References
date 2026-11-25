---
title: "Slicer.TopPixel"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Slicer. Restituisce o imposta lo spostamento verticale della forma slicer dalla sua riga superiore in pixel"
type: docs
url: /it/net/aspose.cells.slicers/slicer/toppixel/
---
## Slicer.TopPixel property

Restituisce o imposta lo spostamento verticale della forma slicer dalla sua riga superiore, in pixel.

```csharp
[Obsolete("Use Shape.Top property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int TopPixel { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Shape.Top. Questa proprietà sarà rimossa 12 mesi dopo, a partire da maggio 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

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
            
            // Crea dati di esempio
            sheet.Cells["A1"].Value = "Product";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 100;
            sheet.Cells["B3"].Value = 200;
            sheet.Cells["B4"].Value = 300;

            // Crea una tabella pivot e ottieni il suo indice
            int pivotIndex = sheet.PivotTables.Add("=A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Aggiungi uno slicer e ottieni il suo indice
            int slicerIndex = sheet.Slicers.Add(pivotTable, "A6", 0);
            Slicer slicer = sheet.Slicers[slicerIndex];
            
            // Imposta la proprietà TopPixel
            slicer.TopPixel = 6;
            
            workbook.Save("SlicerTopPixelDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


