---
title: "Slicer.Placement"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Slicer. Rappresenta il modo in cui l'oggetto di disegno è collegato alle celle sottostanti. La proprietà controlla il posizionamento di un oggetto su un foglio di lavoro."
type: docs
url: /it/net/aspose.cells.slicers/slicer/placement/
---
## Slicer.Placement property

Rappresenta il modo in cui l'oggetto di disegno è collegato alle celle sottostanti. La proprietà controlla il posizionamento di un oggetto su un foglio di lavoro.

```csharp
[Obsolete("Use Shape.Placement property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PlacementType Placement { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà [`Placement`](../../../aspose.cells.drawing/shape/placement/). Questa proprietà sarà rimossa 12 mesi dopo, a partire da gennaio 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Drawing;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyPlacementDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["B4"].Value = 200;

            // Crea una tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");

            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Aggiungi uno slicer per la tabella pivot
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "Fruit", "A6");
            Slicer slicer = worksheet.Slicers[slicerIndex];

            // Imposta le proprietà dello slicer includendo Placement
            slicer.Title = "Fruit Slicer";
            slicer.Placement = PlacementType.MoveAndSize; // Demonstrate Placement property
            slicer.HeightPixel = 200;
            slicer.WidthPixel = 150;

            // Salva la cartella di lavoro
            workbook.Save("SlicerPlacementDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PlacementType](../../../aspose.cells.drawing/placementtype/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


