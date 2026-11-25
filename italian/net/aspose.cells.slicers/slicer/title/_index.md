---
title: "Slicer.Title"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Slicer. Specifica il titolo dell'oggetto Slicer corrente"
type: docs
url: /it/net/aspose.cells.slicers/slicer/title/
---
## Slicer.Title property

Specifica il titolo dell'oggetto Slicer corrente.

```csharp
[Obsolete("Use Shape.Title property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string Title { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà [`Title`](../../../aspose.cells.drawing/shape/title/). Questa proprietà sarà rimossa tra 12 mesi a partire da gennaio 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyTitleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 20;

            // Crea tabella pivot
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "C1", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            pivotTable.CalculateData();

            // Aggiungi slicer
            SlicerCollection slicers = worksheet.Slicers;
            int slicerIndex = slicers.Add(pivotTable, "A1", "Fruit");
            Slicer slicer = slicers[slicerIndex];
            
            // Imposta il titolo dello slicer
            slicer.Title = "Fruit Selection Slicer";
            
            // Salva la cartella di lavoro
            workbook.Save("SlicerTitleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


