---
title: "Slicer.Width"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Slicer. Restituisce o imposta la larghezza dello slicer specificato in punti"
type: docs
url: /it/net/aspose.cells.slicers/slicer/width/
---
## Slicer.Width property

Restituisce o imposta la larghezza dello slicer specificato, in punti.

```csharp
[Obsolete("Use Shape.WidthPt property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double Width { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, utilizza la proprietà Shape.WidthPt. Questa proprietà sarà rimossa 12 mesi dopo, a partire da maggio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyWidthDemo
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
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Crea una tabella pivot
            PivotTableCollection pivotTables = workbook.Worksheets[0].PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Aggiungi uno slicer
            int slicerIndex = worksheet.Slicers.Add(pivotTable, 0, 0, "FruitSlicer");
            Slicer slicer = worksheet.Slicers[slicerIndex];
            
            // Modo corretto per aggiungere la connessione pivot allo slicer
            slicer.AddPivotConnection(pivotTable);

            // Imposta le proprietà dello slicer includendo la larghezza
            slicer.Caption = "Fruit Selection";
            slicer.Width = 150; // Setting the width in points
            slicer.Height = 200;

            // Salva la cartella di lavoro
            workbook.Save("SlicerWidthDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


